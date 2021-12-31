---
title: Tipo de recurso organizationalBrandingLocalization
description: Contém detalhes das localizações de identidade visual da organização.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 847f5271250de49108dfcb7c680847121ea35063
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647011"
---
# <a name="organizationalbrandinglocalization-resource-type"></a>Tipo de recurso organizationalBrandingLocalization

Namespace: microsoft.graph

Recurso que oferece suporte ao gerenciamento de identidade visual específica do idioma. Embora você não possa alterar o idioma da configuração original, esse recurso permite que você crie uma nova configuração para um idioma diferente.

Herda de [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar organizationalBrandingLocalizations](../api/organizationalbranding-list-localizations.md)|coleção [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Obter uma lista dos objetos [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) e suas propriedades.|
|[Criar organizationalBrandingLocalization](../api/organizationalbranding-post-localizations.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Crie um novo [objeto organizationalBrandingLocalization.](../resources/organizationalbrandinglocalization.md)|
|[Obter organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|Leia as propriedades e as relações de um [objeto organizationalBrandingLocalization.](../resources/organizationalbrandinglocalization.md)|
|[Atualizar organizationalBrandingLocalization](../api/organizationalbrandinglocalization-update.md)| Nenhum |Atualize as propriedades de um [objeto organizationalBrandingLocalization.](../resources/organizationalbrandinglocalization.md)|
|[Excluir organizationalBrandingLocalization](../api/organizationalbrandinglocalization-delete.md)|Nenhum|Exclui um [objeto organizationalBrandingLocalization.](../resources/organizationalbrandinglocalization.md)|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| backgroundColor | String | Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda. Recomendamos que você use a cor primária do logotipo da faixa ou da cor da sua organização. Especifique isso no formato hexadecimal, por exemplo, branco é `#FFFFFF` . Herdado [de organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| backgroundImage | Stream | Imagem que aparece como o plano de fundo da página de login. Os tipos permitidos são PNG ou JPEG não menores que 300 KB e não maiores que 1920 × 1080 pixels. Uma imagem menor reduzirá os requisitos de largura de banda e tornará a carga da página mais rápida. Herdado [de organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| backgroundImageRelativeUrl | String | Uma URL relativa para a **propriedade backgroundImage** combinada com uma URL base CDN **cdnList** para fornecer a versão atendida por um CDN. Somente leitura. Herdado [de organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| bannerLogo | Stream | Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada. Os tipos permitidos são PNG ou JPEG não maiores que 36 × 245 pixels. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. Herdado [de organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| bannerLogoRelativeUrl | String | Uma URL relativa para a **propriedade bannerLogo** que é combinada com uma URL base CDN **da cdnList** para fornecer a versão somente leitura atendida por um CDN. Somente leitura. Herdado [de organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| cdnList | Coleção String | Uma lista de URLs base para todos os provedores CDN disponíveis que estão servindo os ativos do recurso atual. Vários CDN provedores são usados ao mesmo tempo para alta disponibilidade de solicitações de leitura. Somente leitura. Herdado [de organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| id | String | Um identificador que representa a localidade especificada usando nomes de cultura. Os nomes de cultura seguem o padrão RFC 1766 no formato "languagecode2-country/regioncode2", onde "languagecode2" é um código de duas letras minúsculo derivado da ISO 639-1 e "country/regioncode2" é um código de duas letras maiúscula derivado da ISO 3166. Por exemplo, inglês dos EUA é `en-US` . A **id para** o padrão /branding é sempre os tipos de cadeia de caracteres `0` ou `default` . Somente leitura. <br/><br/>**OBSERVAÇÃO:** No momento, não há suporte para várias marcas para uma única localidade. Herdado [de organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| signInPageText | String | Texto que aparece na parte inferior da caixa de login. Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal. Este texto deve ser Unicode e não exceder 1024 caracteres. Herdado [de organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| squareLogo | Stream | Uma versão quadrada do logotipo da sua empresa que aparece Windows 10 experiências in-loco (OOBE) e quando o Windows Autopilot está habilitado para implantação. Os tipos permitidos são PNG ou JPEG não maiores que 240 x 240 pixels e no máximo 10 KB de tamanho. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. Herdado [de organizationalBrandingProperties](../resources/organizationalbrandingproperties.md).|
| squareLogoRelativeUrl | String | Uma URL relativa para a **propriedade squareLogo** que é combinada com uma URL base CDN **da cdnList** para fornecer a versão atendida por um CDN. Somente leitura. Herdado [de organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |
| usernameHintText | String | Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada. Este texto deve ser um Unicode, sem links ou código, e não pode exceder 64 caracteres. Herdado [de organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization",
  "baseType": "microsoft.graph.organizationalBrandingProperties",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizationalBrandingLocalization",
  "id": "String (identifier)",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "backgroundImageRelativeUrl": "String",
  "bannerLogo": "Stream",
  "bannerLogoRelativeUrl": "String",
  "cdnList": [
    "String"
  ],
  "signInPageText": "String",
  "squareLogo": "Stream",
  "squareLogoRelativeUrl": "String",
  "usernameHintText": "String"
}
```
