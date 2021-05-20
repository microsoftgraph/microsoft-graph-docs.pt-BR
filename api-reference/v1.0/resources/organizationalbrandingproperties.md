---
title: organalBrandingProperties tipo de recurso
description: Contém detalhes da marca da organização.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 762d2f40cf841c40ce8d7ca6d46337b46343865a
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547271"
---
# <a name="organizationalbrandingproperties-resource-type"></a>organalBrandingProperties tipo de recurso

>[!NOTE]
>Adicionar marca personalizada requer que você use Azure Active Directory Premium 1, Premium 2 ou edições Básicas, ou tenha uma licença Microsoft 365. Para obter mais informações sobre licenciamento e edições, consulte [Inscreva-se no Azure AD Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium).<br><br>As edições Azure AD Premium e Basic estão disponíveis para clientes na China usando a instância mundial de Azure Active Directory. As edições Azure AD Premium e Basic não são atualmente suportadas no serviço Azure operado pela 21Vianet na China. Para mais informações, fale conosco usando o [Fórum Azure Active Directory](https://feedback.azure.com/forums/169401-azure-active-directory/).

Contém detalhes sobre a marca da organização.

As organizações podem personalizar suas páginas de login do Azure AD que aparecem quando os usuários fazem login nos aplicativos específicos de sua organização ou quando o Azure AD identifica o inquilino do usuário a partir de seu nome de usuário. Um desenvolvedor também pode ler as informações de marca da empresa e personalizar sua experiência de aplicativo para adaptá-la especificamente para o usuário conectado usando a marca de sua empresa.

As empresas podem adicionar diferentes marcas com base no local. A localidade serve como chave em todos os pedidos.

>**Nota:** A marca é exposta como uma propriedade sob organização com uma coleção de localizações específicas do local. **organizacionalBrandingProperties** é uma classe abstrata que define propriedades para **o organizacionalBranding**.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/organizationalbrandingproperties-create.md) | [organizaçõesBrandingProperties](organizationalbrandingproperties.md) | Crie marca organizacional com o objeto OrganizationalBrandingProperties. |
| [Get](../api/organizationalbrandingproperties-get.md) | [organizaçõesBrandingProperties](organizationalbrandingproperties.md) | Leia propriedades e relacionamentos do objeto OrganizationalBrandingProperties. |
| [Atualizar](../api/organizationalbrandingproperties-update.md) | [organizaçõesBrandingProperties](organizationalbrandingproperties.md) | Atualizar o objeto OrganizationalBrandingProperties. |
| [Delete](../api/organizationalbrandingproperties-delete.md) | Nenhum | Excluir o objeto organizationalBrandingProperties. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|backgroundColor|Cadeia de caracteres| Cor que aparecerá no lugar da imagem de fundo em conexões de baixa largura de banda. Recomenda-se que a cor principal do logotipo do seu banner ou da sua organização seja usada aqui. Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF). |
|backgroundImage|Stream| Imagem que aparece como o fundo do sinal na página. .png ou .jpg não maior que 1920x1080 e menor que 300kb. Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais executantes. |
|bannerLogo|Stream| Uma versão de banner do logotipo da sua empresa que aparece aparece na página de login. .png ou .jpg não maior que 36x245px. Recomendamos o uso de uma imagem transparente sem estofamento ao redor do logotipo. |
|id|Cadeia de caracteres| Este é um id, herdado do microsoft.graph.entity, é o local especificando o padrão ISO 639 para idioma, por exemplo, o inglês é "en-us" ou "en". Daqui para frente, se expormos a funcionalidade a ter várias marcas para um local, isso pode ser alterado. Observe que o id para Padrão /branding é sempre 'und' até que tenhamos singletons sem chave. Somente leitura. |
|signInPageText|Cadeia de caracteres| Texto que aparece na parte inferior da caixa de entrada. Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal. Este texto deve ser Unicode e não exceder 1024 caracteres. |
|squareLogo|Stream| Versão quadrada do logotipo da sua empresa. Isso aparece em Windows 10 experiências fora da caixa (OOBE) e quando Windows Piloto Automático está habilitado para implantação. .png ou .jpg não maior que 240x240px e não mais do que 10kb de tamanho. Recomendamos o uso de uma imagem transparente sem estofamento ao redor do logotipo. |
|nome de usuárioHintText|Cadeia de caracteres| String que mostra como a dica na caixa de texto do nome de usuário na tela do sinal. Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres. |

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
