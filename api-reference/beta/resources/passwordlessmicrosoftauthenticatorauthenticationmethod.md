---
title: tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Uma representação de um método de entrada de telefone sem senha do autenticador da Microsoft registrado para um usuário.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b34b807106591390198c58d26d7804dc6ada5460
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418206"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type"></a>tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação de um método de entrada de telefone sem senha do autenticador da Microsoft registrado para um usuário.

> [!NOTE]
> Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta. Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md)|coleção [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Recupere uma lista de objetos passwordlessMicrosoftAuthenticatorAuthenticationMethod de um usuário e suas propriedades.|
|[Obter](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md)|[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Leia as propriedades e os relacionamentos do objeto passwordlessMicrosoftAuthenticatorAuthenticationMethod de um usuário.|
|[Excluir](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md)|Nenhum|Exclui o objeto passwordlessMicrosoftAuthenticatorAuthenticationMethod de um usuário.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador do método de autenticação.|
|displayName|Cadeia de caracteres|O nome de exibição do dispositivo móvel conforme fornecido pelo usuário.|
|creationDatetime|DateTimeOffset|O carimbo de data/hora em que esse método foi registrado para o usuário.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)"
}
```

