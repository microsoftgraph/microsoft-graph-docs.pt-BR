---
title: Tipo de recurso windowsApplication
description: Representa configurações para aplicativos que executam o Microsoft Windows e publicados na Microsoft Store ou na loja de jogos do Xbox.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: aricrowe57
ms.openlocfilehash: 9472a8c39a9ddeb7ed7a3857c5bba11c8435d44c
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848675"
---
# <a name="windowsapplication-resource-type"></a>Tipo de recurso windowsApplication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa configurações para aplicativos que executam o Microsoft Windows e publicados na Microsoft Store ou na loja de jogos do Xbox.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| packageSid | Cadeia de caracteres | O identificador de segurança do pacote que a Microsoft atribuiu ao aplicativo. Opcional. Somente leitura. |
| redirectUris | Conjunto de cadeias de caracteres | Especifica as URLs para as quais os tokens de usuário são enviados para entrada ou os URIs de redirecionamento para os quais os códigos de autorização e tokens de acesso do OAuth 2.0 são enviados. Disponível somente para aplicativos que dão suporte à `PersonalMicrosoftAccount` **signInAudience**. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.windowsApplication"
}-->

```json
{
  "packageSid": "String",
  "redirectUris": ["String"]
}

```
