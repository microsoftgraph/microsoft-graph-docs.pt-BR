---
title: Tipo de recurso organizationalBrandingProperties
description: Contém detalhes da identidade visual da organização.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 531e026fa08e13bafc72f0bf361345e7f1d10c0a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158328"
---
# <a name="organizationalbrandingproperties-resource-type"></a>Tipo de recurso organizationalBrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>A adição de identidade visual personalizada exige que você use as edições Azure Active Directory Premium 1, Premium 2 ou Basic ou tenha uma licença do Microsoft 365. Para saber mais sobre licenciamento e edições, confira [Inscrever-se no Azure AD Premium.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)<br><br>As edições Azure AD Premium e Basic estão disponíveis para clientes na China usando a instância mundial do Azure Active Directory. As edições Azure AD Premium e Basic não têm suporte no serviço do Azure operado pela 21Vianet na China. Para obter mais informações, fale conosco usando o Fórum [do Azure Active Directory.](https://feedback.azure.com/forums/169401-azure-active-directory/)

Contém detalhes sobre a identidade visual da organização.

As organizações podem personalizar suas páginas de login do Azure AD que aparecem quando os usuários se ins login em aplicativos específicos do locatário da organização ou quando o Azure AD identifica o locatário do usuário pelo nome de usuário. Um desenvolvedor também pode ler as informações de identidade visual da empresa e personalizar a experiência do aplicativo para adaptá-la especificamente para o usuário assinado usando a identidade visual da empresa.

As empresas podem adicionar identidade visual diferente com base na localidade. A localidade serve como uma chave em todas as solicitações.

>**Observação:** A identidade visual é exposta como uma propriedade na organização com uma coleção de localizações específicas da localidade. **organizationalBrandingProperties** é uma classe abstrata que define propriedades para **organizationalBranding**.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/organizationalbrandingproperties-create.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Crie uma identidade visual organizacional com o objeto organizationalBrandingProperties. |
| [Get](../api/organizationalbrandingproperties-get.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Leia as propriedades e os relacionamentos do objeto organizationalBrandingProperties. |
| [Update](../api/organizationalbrandingproperties-update.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Atualize o objeto organizationalBrandingProperties. |
| [Delete](../api/organizationalbrandingproperties-delete.md) | Nenhum(a) | Exclua o objeto organizationalBrandingProperties. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|backgroundColor|String| Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda. A cor principal do logotipo da faixa ou da cor da organização é recomendada para ser usada aqui. Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF). |
|backgroundImage|Stream| Imagem que aparece como o plano de fundo da página de login. .png ou .jpg não maior que 1920x1080 e menor que 300kb. Uma imagem menor reduzirá os requisitos de largura de banda e fará com que as cargas de página se realizem com mais desempenho. |
|bannerLogo|Stream| Uma versão em faixa do logotipo da empresa que aparece na página de entrada. .png ou .jpg não maior que 36x245px. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. |
|id|String| Essa é uma id, herdada de microsoft.graph.entity, é a localidade que especifica o padrão ISO 639 para idioma, por exemplo, inglês é "en-us" ou "en". No futuro, se expormos a funcionalidade para ter várias identidade visual para uma localidade, isso poderá ser alterado. Observe que a ID de Default /branding é sempre 'und' até termos singletons sem teclas. Somente leitura. |
|signInPageText|String| Texto que aparece na parte inferior da caixa de login. Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal. Esse texto deve ser Unicode e não exceder 1024 caracteres. |
|squareLogo|Stream| Versão quadrada do logotipo da empresa. Isso aparece nas experiências do Windows 10 (OOBE) e quando o Windows Autopilot está habilitado para implantação. .png ou .jpg com no máximo 240 x 240px e no máximo 10kb de tamanho. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. |
|usernameHintText|String| Cadeia de caracteres que é a dica na caixa de texto do nome de usuário na tela de entrada. Esse texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationalBrandingProperties",
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
