Kütüphanelerin Kurulumu
=======================

Bu Python kodunun çalışması için aşağıdaki kütüphanelerin kurulu olması gerekmektedir:

*   os
*   shutil
*   random
*   json
*   glob
*   win32com.client
*   PIL (Pillow kütüphanesini içerir)
*   requests
*   reportlab

Kütüphaneleri kurmak için aşağıdaki komutları kullanabilirsiniz:

    pip install Pillow
    pip install requests
    pip install reportlab

Ayrıca, Windows işletim sistemine sahipseniz `pywin32` kütüphanesini yüklemeniz gerekebilir:

    pip install pywin32

Kodun Çalıştırılması
====================

Kodu çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1.  Gerekli kütüphanelerin kurulu olduğundan emin olun.
2.  Kodu bir Python dosyasına yapıştırın (örneğin, `main.py`).
3.  `ayarlar.json` adında bir yapılandırma dosyası oluşturun ve içine aşağıdaki gibi ayarları ekleyin:

    {
      "input_folder": "input_folder_path",
      "mockup_folder": "mockup_folder_path",
      "action_name": "action_name",
      "action_set_name": "action_set_name",
      "keywords": ["keyword1", "keyword2", "keyword3"],
      "min_mockup_files": 1,
      "max_mockup_files": 3,
      "go_file_token": "your_gofile_token"
    }

**"input\_folder"**: İşlenecek görüntülerin bulunduğu klasörün yolunu belirtin.

**"mockup\_folder"**: Mockup görüntülerinin bulunduğu klasörün yolunu belirtin.

**"action\_name"**: Photoshop eyleminin adını belirtin.

**"action\_set\_name"**: Photoshop eylem kümesinin adını belirtin.

**"keywords"**: Eylem sonucunda oluşturulan dosya adları için kullanılacak anahtar kelimeleri belirtin.

**"min\_mockup\_files"**: Kopyalanacak en az mockup dosyası sayısını belirtin.

**"max\_mockup\_files"**: Kopyalanacak en fazla mockup dosyası sayısını belirtin.

**"go\_file\_token"**: Gofile.io API'si için kullanılacak token'ı belirtin.

4.  `input_folder_path` ve `mockup_folder_path` değerlerini gerçek klasör yollarıyla değiştirin.
5.  `action_name` ve `action_set_name` değerlerini Photoshop'ta mevcut olan eylem ve eylem kümesi adlarıyla değiştirin.
6.  `"keywords"` listesine istediğiniz anahtar kelimeleri ekleyin.
7.  `"go_file_token"` değerini Gofile.io hesabınızın API token'ıyla değiştirin.
8.  Kaydedin ve dosyayı çalıştırın: `python main.py`.

Kod, belirtilen yapılandırmaya göre işlenecek görüntülerin kopyalanması, yeniden adlandırılması, yeniden boyutlandırılması, mockup dosyalarının kopyalanması, Photoshop eyleminin uygulanması, dosyaların Gofile.io'ya yüklenmesi ve PDF indirme bağlantılarının oluşturulması gibi işlemleri gerçekleştirecektir.


English:
 Python Code Description

Library Installation
====================

The following libraries need to be installed for this Python code to work:

*   os
*   shutil
*   random
*   json
*   glob
*   win32com.client
*   PIL (includes the Pillow library)
*   requests
*   reportlab

You can install the libraries using the following commands:

    pip install Pillow
    pip install requests
    pip install reportlab

If you are using Windows operating system, you may need to install the \`pywin32\` library:

    pip install pywin32

Running the Code
================

Follow the steps below to run the code:

1.  Make sure the required libraries are installed.
2.  Paste the code into a Python file (e.g., \`main.py\`).
3.  Create a configuration file named \`settings.json\` and add the following settings:

    {
      "input_folder": "input_folder_path",
      "mockup_folder": "mockup_folder_path",
      "action_name": "action_name",
      "action_set_name": "action_set_name",
      "keywords": ["keyword1", "keyword2", "keyword3"],
      "min_mockup_files": 1,
      "max_mockup_files": 3,
      "go_file_token": "your_gofile_token"
    }

**"input\_folder"**: Specify the path to the folder containing the images to be processed.

**"mockup\_folder"**: Specify the path to the folder containing the mockup images.

**"action\_name"**: Specify the name of the Photoshop action.

**"action\_set\_name"**: Specify the name of the Photoshop action set.

**"keywords"**: Specify the keywords to be used for generating file names.

**"min\_mockup\_files"**: Specify the minimum number of mockup files to be copied.

**"max\_mockup\_files"**: Specify the maximum number of mockup files to be copied.

**"go\_file\_token"**: Specify the token for Gofile.io API.

4.  Replace \`input\_folder\_path\` and \`mockup\_folder\_path\` values with the actual folder paths.
5.  Replace \`action\_name\` and \`action\_set\_name\` values with the existing action and action set names in Photoshop.
6.  Add your desired keywords to the \`"keywords"\` list.
7.  Replace \`"go\_file\_token"\` value with your Gofile.io API token.
8.  Save the file and run it: \`python main.py\`.

The code will perform operations such as copying, renaming, resizing images, copying mockup files, applying Photoshop actions, uploading files to Gofile.io, and generating PDF download links based on the specified configuration.
