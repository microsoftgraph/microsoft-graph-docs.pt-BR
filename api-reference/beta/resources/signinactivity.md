---
title: Tipo de recurso signInActivity
description: Fornece a última hora de login interativa ou não interativa para um usuário específico.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c67966902315f4b8ef4ab75f7f0c8d3cb5988f98
ms.sourcegitcommit: 9759b647acfbed99d5675a6f512aaa33932a723f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/23/2021
ms.locfileid: "61604179"
---
# <a name="signinactivity-resource-type"></a>Tipo de recurso signInActivity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece a última hora de login interativa ou não interativa para um usuário [específico.](user.md) Como signInActivity descreve uma propriedade do objeto do usuário, o Azure AD armazena a signinatividade para seus usuários desde que os objetos do usuário existam. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|lastSignInDateTime|DateTimeOffset|A última data e hora interativas de login para um usuário específico. Você pode usar esse campo para calcular a última vez que um usuário se inscreveu no diretório com um método de autenticação interativa. Esse campo pode ser usado para criar relatórios, como usuários inativos. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é: `'2014-01-01T00:00:00Z'` . O Azure AD mantém as inscrições interativas que vão voltar para abril de 2020. Para obter mais informações sobre como usar o valor dessa propriedade, consulte Gerenciar contas de usuário [inativas no Azure AD](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).|
|lastSignInRequestId|Cadeia de caracteres|Identificador de solicitação do último login interativo executado por esse usuário.|
|lastNonInteractiveSignInDateTime|DateTimeOffset|A última data de login não interativa para um usuário específico. Você pode usar esse campo para calcular a última vez que um cliente se inscreveu no diretório em nome de um usuário. Como alguns usuários podem usar clientes para acessar recursos de locatário em vez de entrar diretamente no locatário, você pode usar a data de entrada não interativa para junto com lastSignInDateTime para identificar usuários inativos. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é: `'2014-01-01T00:00:00Z'` . O Azure AD mantém as inscrições não interativas que vão voltar para maio de 2020. Para obter mais informações sobre como usar o valor dessa propriedade, consulte Gerenciar contas de usuário [inativas no Azure AD](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).|
|lastNonInteractiveSignInRequestId|Cadeia de caracteres|Identificador de solicitação da última assinatura não interativa realizada por esse usuário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInActivity",
  "baseType": null
}-->

```json
{
  "lastSignInDateTime": "String (timestamp)",
  "lastSignInRequestId": "String",
  "lastNonInteractiveSignInDateTime": "String (timestamp)",
  "lastNonInteractiveSignInRequestId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
