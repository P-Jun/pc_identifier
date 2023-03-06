[폴더 위치]
licensecc insall 후 해당 폴더에 위치 시켜주세요
cd ./licensecc/install

[동작법]
cd pc_identifier/build 
cmake .. -Dlicensecc_DIR={install 폴더}/cmake/licensecc
./pc_identifier.exe

[error]
경로 지정할 때 상대경로로 지정하면 폴더를 찾지 못하는 에러가 발생할 수 있습니다. 해당 경우 경로를 절대 경로로 지정해주면 됩니다.
때에 따라 licensecc의 cmake의 파일명이 다를 수 있습니다. licensecc의 내부 구현체 설명을 따라 "licenseccConfig.cmake"이나 "licensecc-config.cmake"을 찾아서 -Dlicensecc_DIR로 지정해주면 됩니다.

id를 얻고, 하드웨어의 라이선스 확인은 구현된 identify_pc API를 사용하여 자세한 사항은 공식 문서를 확인해 주시길 바랍니다.
http://open-lic
