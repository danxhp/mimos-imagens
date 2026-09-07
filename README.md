# mimos-imagens

Hospedagem das imagens de produto usadas na exportação do Bling para os marketplaces.

**Por que existe:** o Bling baixa a URL da imagem e a envia ao canal no momento da exportação.
As URLs originais do CDN da Rommanel falham nesse momento — 52% já respondem 404, e mesmo as
que respondem 200 para um navegador não foram baixadas pelo Bling. Sem imagem, a exportação
é recusada.

**A hospedagem é transitória.** Depois que a exportação conclui, o Bling guarda a imagem
internamente e o canal também — a URL de origem pode cair sem afetar o anúncio. O primeiro
anúncio da loja está no ar até hoje com as URLs originais em 404.

Estrutura: `img/<sku>/<sku>_<n>.jpg`
