            
            
            //bancodeimagens
            let imagens = [
                "https://t.ctcdn.com.br/93b35I56edm3bcmuCoRvK3xSBOk=/62x74:1213x722/640x360/smart/i335995.jpeg",
                "https://t.ctcdn.com.br/6BSSH8Hcd3M1qjljj249YXCJ0bw=/660x0/smart/i494623.jpeg", 
                "https://t.ctcdn.com.br/93b35I56edm3bcmuCoRvK3xSBOk=/62x74:1213x722/640x360/smart/i335995.jpeg",
                "https://img.canaltech.com.br/canaltech-icon.svg",
                "https://t.ctcdn.com.br/pSgq84YkapE0D4jYHHF75qTkIVQ=/1024x0/smart/i494613.jpeg",
                "https://t.ctcdn.com.br/XHx7SwLeTfMkOFlIkHVtRXRmlog=/1024x0/smart/i494616.png",
                "https://src.trvdp.com/images/310c9de922672c4aa4b8e11e7768c513e88d8646_2.jpg",
                "https://ads.stickyadstv.com/auto-user-sync?_fw_gdpr=0&_fw_gdpr_consent=",
                "https://ads.stickyadstv.com/user-matching?id=2545&_fw_gdpr=0&_fw_gdpr_consent=",
                "https://t.ctcdn.com.br/6BSSH8Hcd3M1qjljj249YXCJ0bw=/660x0/smart/i494623.jpeg",
                "https://t.ctcdn.com.br/RkJ6SRPW04lAm-ADivn97ralS0E=/660x0/smart/i494621.png",
                "https://t.ctcdn.com.br/yQjzwXSoVEGiySB0OWfeKSoxzfY=/660x0/smart/i494615.jpeg",
                "https://t.ctcdn.com.br/05N5tgdXlkIPyhJa_wt6Bn8fpp0=/1024x0/smart/i494617.png",
                "https://conteudo.imguol.com.br/c/noticias/88/2022/03/14/colisao-de-bicicletas-1647266693556_v2_1920x1920.jpg.webp",
                "https://conteudo.imguol.com.br/c/noticias/d1/2022/03/14/eu-consigo-voar-1647266691666_v2_150x150.jpg.webp",
                "https://conteudo.imguol.com.br/c/noticias/06/2022/03/14/darth-vader-tambem-tira-o-lixo-1647266690151_v2_150x150.jpg.webp",
                "https://conteudo.imguol.com.br/c/noticias/08/2022/03/14/vamos-observar-o-ceu-no-meio-da-estrada-1647266685722_v2_150x150.png.webp",
                "https://conteudo.imguol.com.br/c/noticias/ae/2022/03/14/batman-prestes-a-entrar-em-acao-1647266677434_v2_150x150.jpg.webp",
                "https://conteudo.imguol.com.br/c/noticias/0c/2022/03/14/algo-de-errado-nao-esta-certo-1647266672886_v2_150x150.png.webp",
                "https://conteudo.imguol.com.br/c/noticias/42/2022/03/14/clones-de-luxo-1647266658135_v2_150x150.png.webp",
                "https://conteudo.imguol.com.br/c/noticias/96/2022/03/14/exposicao-de-manequins-1647266653345_v2_150x150.png.webp",
                "https://conteudo.imguol.com.br/c/noticias/73/2022/03/14/e-caiu-1647266652163_v2_150x150.jpg.webp",
                "https://conteudo.imguol.com.br/c/geral/3d/2021/05/25/placeholder-image-1621949831997_v2_300x225.jpg",
                "https://conteudo.imguol.com.br/c/geral/3d/2021/05/25/placeholder-image-1621949831997_v2_300x225.jpg",
                "https://conteudo.imguol.com.br/c/geral/3d/2021/05/25/placeholder-image-1621949831997_v2_300x225.jpg",
                "https://conteudo.imguol.com.br/c/geral/3d/2021/05/25/placeholder-image-1621949831997_v2_300x225.jpg",
                "https://conteudo.imguol.com.br/c/geral/3d/2021/05/25/placeholder-image-1621949831997_v2_300x225.jpg",
                "https://conteudo.imguol.com.br/c/geral/3d/2021/05/25/placeholder-image-1621949831997_v2_300x225.jpg",
                "https://conteudo.imguol.com.br/c/geral/3d/2021/05/25/placeholder-image-1621949831997_v2_300x225.jpg",
                "https://conteudo.imguol.com.br/c/geral/3d/2021/05/25/placeholder-image-1621949831997_v2_300x225.jpg",
                "https://conteudo.imguol.com.br/c/geral/3d/2021/05/25/placeholder-image-1621949831997_v2_300x225.jpg",
                "https://conteudo.imguol.com.br/c/geral/3d/2021/05/25/placeholder-image-1621949831997_v2_300x225.jpg",
                "https://conteudo.imguol.com.br/c/noticias/84/2022/06/23/retrato-solar-1656018906008_v2_300x225.jpg.webp",
                "https://conteudo.imguol.com.br/c/noticias/eb/2022/06/15/superlua-de-morango-sobre-o-templo-de-posseidon-proximo-a-atenas-na-grecia-1655296577157_v2_300x225.jpg.webp",
                "https://conteudo.imguol.com.br/c/noticias/54/2022/05/30/carnotauro-recriado-em-cgi-para-a-serie-documentarial-prehistoric-planet-da-appletv-1653914008445_v2_300x225.jpg.webp"
                // Adicione mais URLs se quiser
                
            ];
            //logicadagaleriadeimagens
            let galeria = document.getElementById('galeria');
            let botao = document.getElementById('btn');
            let indice = 0;
            let limite = 1;

            botao.onclick = function () {
                let final = indice + limite;

                for (; indice < final && indice < imagens.length; indice++) {
                    let imagem = document.createElement('img');
                    imagem.width = 300;
                    imagem.height = 300;
                    imagem.src = imagens[indice];
                    galeria.appendChild(imagem);
                }

                if (indice >= imagens.length) {
                    botao.disabled = true;
                    botao.textContent = 'Desativado';
                }
                //logicadagaleriadeimagens
            };

