---
title: Tipo de recurso certificateBasedAuthConfiguration
description: Representa uma coleção de autoridades de certificados.
ms.localizationpriority: medium
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 53e56f78508131e3a08e7896095a7f986346fba2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104254"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a>Tipo de recurso certificateBasedAuthConfiguration

Namespace: microsoft.graph

A autenticação baseada em certificado permite que você seja autenticado pelo Azure Active Directory com um certificado de cliente em um dispositivo Windows, Android ou iOS ao conectar sua conta Exchange Online a:

- Aplicativos móveis da Microsoft, como o Outlook e o Word
- Clientes do Exchange ActiveSync (EAS)

A configuração desse recurso elimina a necessidade de inserir uma combinação de nome de usuário e senha em determinados aplicativos de email e Microsoft Office em seu dispositivo móvel.

A configuração de autenticação baseada em certificado é fornecida por meio de uma coleção de autoridades de certificados. As autoridades de certificados são usadas para estabelecer uma cadeia de certificados confiável que permite que os clientes sejam autenticados por Azure Active Directory com um certificado de cliente.

Saiba mais sobre [autenticação baseada em certificado em Azure Active Directory](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-list.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | Listar as propriedades da **coleção certificateBasedAuthConfiguration.** |
| [Criar certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | Crie um novo **objeto certificateBasedAuthConfiguration.** |
| [Obter certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-get.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | Leia as propriedades de **um objeto certificateBasedAuthConfiguration.** |
| [Excluir certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-delete.md) | Nenhum(a) | **Exclua um objeto certificateBasedAuthConfiguration.** |

>[!NOTE]
>Não há suporte para a atualização de **certificateBasedAuthConfiguration.** Para alterar **um certificateBasedAuthConfiguration,** primeiro exclua e crie um novo **certificateBasedAuthConfiguration**.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|certificateAuthorities|[Coleção certificateAuthority](certificateauthority.md)|Coleção de autoridades de certificados que cria uma cadeia de certificados confiável.|
|id|Cadeia de caracteres|O identificador exclusivo da configuração de auth baseada em certificado. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum,

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "keyProperty": "id"
}-->

```json
{
  "certificateAuthorities": {"@odata.type": "collection(microsoft.graph.certificateAuthority)"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateBasedAuthConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
