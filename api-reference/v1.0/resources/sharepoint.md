# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a>Trabalhar com sites do SharePoint no Microsoft Graph

A API do SharePoint no Microsoft Graph suporta os seguintes cenários principais:

* Acesso aos **sites** e às **unidades** do SharePoint (bibliotecas de documentos)
* Suporte somente leitura para recursos de **site** (nenhuma capacidade de criar novos sites)
* Suporte a leitura e gravação **driveItems**
* Lidar com recursos por ID do SharePoint, URL ou caminho relativo

## <a name="sharepoint-api-root-resources"></a>Recursos de raiz da API do SharePoint

Os exemplos a seguir são relativos a `https://graph.microsoft.com/v1.0`.

| Caminho                                   | Descrição
|:---------------------------------------|:------------------------------------
| /sites/root                            | [Site][] padrão da organização.
| /sites/{site-id}                       | Acessar um [site][] específico por sua identificação.
| /sites/{site-id}/drive                 | Acessar a [unidade](drive.md) padrão (biblioteca de documentos) desse [site][].
| /sites/{site-id}/drives                | Enumerar as [unidades](drive.md) (bibliotecas de documentos) no [site][].
| /sites/{site-id}/sites                 | Enumerar os subsites no [site][].
| /groups/{group-id}/sites/root          | Acesse um [site][] de equipe do grupo.

Sites também podem ser tratados pelo caminho usando o nome de host do SharePoint, seguido por dois pontos e o caminho relativo para o site. Opcionalmente, você pode fazer a transição para lidar com o modelo de recurso colocando outros dois pontos no final.

| Caminho                                           | Descrição
|:-----------------------------------------------|:-----------------------------------
| /sites/contoso.sharepoint.com:/teams/hr        | O site associado a https://contoso.sharepoint.com/teams/hr
| /sites/contoso.sharepoint.com:/teams/hr:/drive | Acessar a [unidade](drive.md) padrão desse.

## <a name="note-for-existing-sharepoint-developers"></a>Observação para desenvolvedores do SharePoint existentes

A API do Microsoft Graph do SharePoint tem algumas diferenças essenciais das APIs CSOM. Os recurso do [site][] mapeia para `SPWeb`. O [site][] (`SPWeb`) raiz em uma coleção de site com uma faceta [siteCollection](sitecollection.md), que contém informações sobre o `SPSite`. Como as IDs de sites são exclusivas penas em sua coleção de site, abordar um site por ID requer o fornecimento do identificador de coleção de site e identificador de site.

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id},{spweb-id}/
```
Uma URL construída com apenas o nome do host apontará para o site raiz (`SPWeb`) na coleção de sites padrão.

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname}
```

Uma URL construída apenas com o nome do host e ID de siteCollection (`SPSite`) apontará o site raiz (`SPWeb`) na coleção de sites determinada.

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id}
```

[site]: site.md
[drive]: drive.md
[siteCollection]: siteCollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->
