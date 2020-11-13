---
title: tipo de recurso organizationalBrandingProperties
description: Contém detalhes da identidade visual da organização.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b96d4453f07ce317eb41902ed33282d961c74f16
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031889"
---
# <a name="organizationalbrandingproperties-resource-type"></a>tipo de recurso organizationalBrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>A adição de identidade visual personalizada requer que você use as edições 1, Premium 2 ou básica do Azure Active Directory, ou tenha uma licença do Microsoft 365. Para obter mais informações sobre licenciamento e edições, consulte [inscrever-se no Azure ad Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium).<br><br>O Azure AD Premium e edições básicas estão disponíveis para clientes da China usando a instância Mundial do Azure Active Directory. Atualmente, o Azure AD Premium e o Basic Edition não têm suporte no Azure Service operado pela 21Vianet na China. Para obter mais informações, fale conosco usando o [Fórum do Azure Active Directory](https://feedback.azure.com/forums/169401-azure-active-directory/).

Contém detalhes sobre a identidade visual da organização.

As organizações podem personalizar suas páginas de entrada do Azure AD que aparecem quando os usuários entram nos aplicativos específicos de locatários da sua organização, ou quando o Azure AD identifica o locatário do usuário de seu nome de usuário. Um desenvolvedor também pode ler as informações de identidade visual da empresa e personalizar sua experiência de aplicativo para ajustá-la especificamente para o usuário conectado usando a identidade visual da empresa.

As empresas podem adicionar diferentes identidade visual com base na localidade. A localidade serve como uma chave em todas as solicitações.

>**Observação:** A identidade visual é exposta como uma propriedade em organização com uma coleção de localizações específicas de localidade. **organizationalBrandingProperties** é uma classe abstrata que define propriedades para **organizationalBranding**.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Create](../api/organizationalbrandingproperties-create.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Crie uma identidade visual organizacional com o objeto organizationalBrandingProperties. |
| [Get](../api/organizationalbrandingproperties-get.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Leia as propriedades e os relacionamentos do objeto organizationalBrandingProperties. |
| [Atualização](../api/organizationalbrandingproperties-update.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Atualize o objeto organizationalBrandingProperties. |
| [Delete](../api/organizationalbrandingproperties-delete.md) | Nenhum | Exclua o objeto organizationalBrandingProperties. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|CorDoFundo|String| Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda. É recomendável usar a cor principal do logotipo de faixa ou a cor da sua organização aqui. Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF). |
|backgroundImage|Fluxo| Imagem que aparece como plano de fundo da página de entrada. . png ou. jpg não é maior do que 1920 x 1080 e menor do que 300kb. Uma imagem menor reduzirá os requisitos de largura de banda e fará com que as cargas de página mais tenham mais desempenho. |
|bannerLogo|Fluxo| Uma versão de banner do logotipo da empresa que aparece aparece na página de entrada. . png ou. jpg não maior do que 36x245px. Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo. |
|id|String| É uma ID, herdada de Microsoft. Graph. Entity, é a localidade que especifica o padrão ISO 639 para o idioma, por exemplo, inglês (en-US) ou "en". Encaminhar se exportarmos funcionalidade para ter várias marcas para uma localidade, isso pode ser alterado. Observe que a ID do/branding padrão é sempre ' und ' até que haja singleton. Somente leitura. |
|signInPageText|String| Texto que aparece na parte inferior da caixa de entrada. Você pode usá-lo para comunicar informações adicionais, como o número de telefone para o suporte técnico ou uma instrução legal. Este texto deve ser Unicode e não exceder 1024 caracteres. |
|squareLogo|Fluxo| Versão quadrada do logotipo da sua empresa. Isso aparece nas experiências de uso (OOBE) do Windows 10 e quando o Windows AutoPilot está habilitado para implantação. . png ou. jpg não maior do que 240x240px e não mais do que 10 KB em tamanho. Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo. |
|usernameHintText|String| Cadeia de caracteres que mostra como a dica na caixa de texto username na tela de entrada. Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationalBrandingProperties",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "id": "String (identifier)",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationalBrandingProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
