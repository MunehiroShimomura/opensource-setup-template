aitrios-edge-device-build-linux/
������ t4-otoblite/
��  ������ yocto-bsp/		# 
��  	������ meta-xxx-boot
��  	������ meta-edge-device-core (s)
������ t4-refsys/
��  ������ yocto-bsp/		# 




edge-device-core-yocto/
  meta-edge-device-core-base
  meta-edge-device-core-nxp
  meta-edge-device-core-broadcom


or

aitrios-edge-device-build-linux/
������ t4
��  ������ yocto-bsp/		# 

or 

aitrios-edge-device-build/
 ������ t4-otoblite/
 ������ t4-refsys/
 ������ t3p/
 ������ t3pw/
 ������ t5/


--------------------------------
edge-device-core/
������ src/			# �\�[�X�R�[�h
��  ������ include/		# edge-device-core�S�̂�include.�Ȃ���������Ȃ�
��  ������ manager/		# manager�i�[�p
��  ��  ������ led/		# led manager
��  ��  ��  ������ include/	# 
��  ��  ��  ������ hal/		# ����̍\����manager�̉���hal������H
��  ��  ������ net/		# �K�v�Ȋemanager�B�t�H���_�\����led���l
��  ��  ������ xxx/
��  ��  ������ yyy/
��  ������ app/			# Sysapp�֘A
��  ��  ������ sysapp/		# 
��  ��  ������ initapp/		# 
��  ������ senscord/		# subproject? or conan, vcpkg�Ȃǎg���������ǂ�����
��  ������ evp/			# subproject? or conan, vcpkg�Ȃǎg���������ǂ�����  �N���X�R���p�C���Ή����Ăق��� cmake?
������ external/
��  ������ wamr/		# subproject? or conan, vcpkg�Ȃǎg���������ǂ��H�� cont back����Ȃ�submodule�����₷���H
��  ������ ...			# 
������ build/                   # �r���h�pscript
��   ������ debian		# Rasp-pi�����Bdeb�p�b�P�[�W�����܂�
������ doc/			# �h�L�������g�i�d�l���AAPI���t�@�����X�Ȃǁj
������ tool/			# �J����r���h�ɕK�v�ȃc�[���Ȃ�
������ script/			# �C���X�g�[���ŕK�v��script�������
������ test/			# �e�X�g�ɕK�v�Ȉꎮ�B�e�X�g�x���`�A�e�X�g�f�[�^�A�e�X�g�V�i���I��
������ Makefile			# make master (Cmake�����Ȃ�CmakeLists.txt��)
������ Makefile.config		# make master (Cmake�����Ȃ�CmakeLists.txt��)
������ README.md
������ LICENSE			# �Ώە��̃��C�Z���X�̖���
������ CONTRIBUTING.md		# �R���g���r���[�V�����̃K�C�h
������ CODE_OF_CONDUCT.md	# �s���K�́E�R���g���r���[�V���������̈����錾
������ SECURITY.md 		# �Z�L�����e�B�ɑ΂���s���K�́E�K�C�h
������ PULL_REQUEST_TEMPLATE.md	# Pull Req���̃e���v���[�g  .github��������
������ ISSUE_TEMPLATE.md�@�@�@�@#.github��������
������ CODEOWNERS
������ CHANGES.md





edge-device-core.deb
  - libwamr.so
  - libsenscord.so
  - libevp.so
  - libesf.so
  - sysapp

json.deb
  - libjson.so

jpeg.deb
  - libjpeg.so

