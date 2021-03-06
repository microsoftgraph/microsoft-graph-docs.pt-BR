---
title: Tipo de recurso organizationalBrandingProperties
description: Contém detalhes da identidade visual da organização.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e27966381c5838ac7662b977c5061a46bb660f1c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442912"
---
# <a name="organizationalbrandingproperties-resource-type"></a>Tipo de recurso organizationalBrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>Adicionar identidade visual personalizada exige que você use edições do Azure Active Directory Premium 1, Premium 2 ou Basic ou ter uma licença do Microsoft 365. Para obter mais informações sobre licenciamento e edições, [consulte Inscrever-se no Azure AD Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium).<br><br>As edições Azure AD Premium e Basic estão disponíveis para clientes na China usando a instância mundial do Azure Active Directory. As edições Do Azure AD Premium e Basic não têm suporte no serviço do Azure operado pela 21Vianet na China. Para obter mais informações, fale conosco usando o [Fórum do Azure Active Directory](https://feedback.azure.com/forums/169401-azure-active-directory/).

Contém detalhes sobre a identidade visual da organização.

As organizações podem personalizar suas páginas de login do Azure AD que aparecem quando os usuários entrar nos aplicativos específicos do locatário da organização ou quando o Azure AD identifica o locatário do usuário do nome de usuário. Um desenvolvedor também pode ler as informações de identidade visual da empresa e personalizar sua experiência de aplicativo para adaptá-la especificamente para o usuário que está assinado usando a identidade visual da empresa.

As empresas podem adicionar identidade visual diferente com base na localidade. A localidade serve como uma chave em todas as solicitações.

>**Observação:** A identidade visual é exposta como uma propriedade sob organização com uma coleção de localizações específicas da localidade. **organizationalBrandingProperties** é uma classe abstrata que define propriedades para **organizationalBranding**.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/organizationalbrandingproperties-create.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Criar identidade visual organizacional com o objeto organizationalBrandingProperties. |
| [Get](../api/organizationalbrandingproperties-get.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Leia propriedades e relações do objeto organizationalBrandingProperties. |
| [Atualização](../api/organizationalbrandingproperties-update.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Atualizar o objeto organizationalBrandingProperties. |
| [Delete](../api/organizationalbrandingproperties-delete.md) | Nenhum(a) | Exclua o objeto organizationalBrandingProperties. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|backgroundColor|String| Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda. A cor primária do logotipo da faixa ou da cor da sua organização é recomendada para ser usada aqui. Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF). |
|backgroundImage|Stream| Imagem que aparece como o plano de fundo da página de logom. .png ou .jpg não maior que 1920x1080 e menor que 300kb. Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais performant. |
|bannerLogo|Stream| Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada. .png ou .jpg não maior que 36x245px. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. |
|id|String| Esta é uma id, herdada de microsoft.graph.entity, é a localidade que especifica o padrão ISO 639 para idioma, por exemplo, inglês é "en-us" ou "en". Daqui para frente, se expormos a funcionalidade para ter várias marcas para uma localidade, isso poderá ser alterado. Observe que id para Padrão /identidade visual é sempre 'und' até termos singletons sem teclas. Somente leitura. |
|signInPageText|String| Texto que aparece na parte inferior da caixa de login. Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal. Este texto deve ser Unicode e não exceder 1024 caracteres. |
|squareLogo|Stream| Versão quadrada do logotipo da sua empresa. Isso aparece nas experiências OOBE (windows 10 out-of-box) e quando o Windows Autopilot está habilitado para implantação. .png ou .jpg não maior do que 240x240px e no máximo 10kb de tamanho. Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo. |
|usernameHintText|String| Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada. Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres. |

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
