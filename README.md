[폴더 위치]<br>
licensecc insall 후 해당 폴더에 위치 시켜주세요<br>
cd ./licensecc/install<br>
<br>
[동작법]<br>
cd pc_identifier/build <br>
cmake .. -Dlicensecc_DIR={install 폴더}/cmake/licensecc<br>
./pc_identifier.exe<br>
<br>
[error]<br>
경로 지정할 때 상대경로로 지정하면 폴더를 찾지 못하는 에러가 발생할 수 있습니다. 해당 경우 경로를 절대 경로로 지정해주면 됩니다.<br>
때에 따라 licensecc의 cmake의 파일명이 다를 수 있습니다. licensecc의 내부 구현체 설명을 따라 "licenseccConfig.cmake"이나 "licensecc-config.cmake"이 존재하는 폴더를 찾아서 -Dlicensecc_DIR로 지정해주면 됩니다.<br>
<br>
id를 얻고, 하드웨어의 라이선스 확인은 구현된 identify_pc API를 사용하여 자세한 사항은 [공식 문서](http://open-license-manager.github.io/licensecc/api/public_api.html#print-hardware-identifier)를 확인해 주시길 바랍니다.<br>
