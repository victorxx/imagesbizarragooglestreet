from playwright.sync_api import sync_playwright

with sync_playwright() as p:
    browser = p.chromium.launch(headless=False)
    page = browser.new_page()
    urls = []

    # Acessa a página
    page.goto(
        'https://www.uol.com.br/tilt/album/2022/03/28/perolas-google-maps.htm',
        timeout=50000
    )
    
    # Rola a página para baixo para carregar imagens que usam lazy loading
    for _ in range(5):
        page.mouse.wheel(0, 1000)
        page.wait_for_timeout(1500)  # Aguarda o carregamento das imagens visíveis

    # Coleta todos os elementos <img> da página
    imagens = page.locator('img').element_handles()

    # Extensões válidas para imagens
    extensoes_validas = ('.png', '.jpeg', '.jpg', '.gif', '.bmp', '.webp')

    # Extrai os atributos src das imagens e filtra pelas extensões
    for img in imagens:
        src = img.get_attribute('src')
        if src and src.lower().endswith(extensoes_validas):
            urls.append(f'"{src}"')  # Ou sem aspas: urls.append(src)

    # Junta as URLs com vírgula ou apenas exibe uma por linha
    final = ',\n '.join(urls)
    print(final)
    with open(r'C:\Users\vitor\Desktop\imagenslinks.txt','a+', encoding='utf-8') as file:
        file.write(final)

    # Fecha o navegador
    browser.close()
