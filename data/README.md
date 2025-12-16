# Скачать файл Sample_Superstore.csv
[Kaggle Dataset(сайт)](https://www.kaggle.com/datasets/htagholdings/property-sales/data?select=raw_sales.csv) / [Kaggle Dataset(github)](hause_sales.csv)
# Использовать выгрузку с kaggle(необходимо наличие токена):
    !pip install kaggle
    os.environ['KAGGLE_CONFIG_DIR'] = '/content/drive/MyDrive/kaggle'
    ! kaggle datasets download htagholdings/property-sales
    file_path = '/content/property-sales.zip'
    with zipfile.ZipFile(file_path, 'r') as zip_ref:
        zip_ref.extractall('/content')
    df = pd.read_csv('raw_sales.csv')
