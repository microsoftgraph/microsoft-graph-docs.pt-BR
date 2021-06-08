---
title: Tipo de recurso provisionChannelEmailResult
description: Representa o resultado de uma operação de provisionamento de email de canal.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac32dd0db4877dc01a13536689d414b0dcc1175f
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813221"
---
# <a name="provisionchannelemailresult-resource-type"></a><span data-ttu-id="96ff9-103">Tipo de recurso provisionChannelEmailResult</span><span class="sxs-lookup"><span data-stu-id="96ff9-103">provisionChannelEmailResult resource type</span></span>

<span data-ttu-id="96ff9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96ff9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96ff9-105">Representa o endereço de email [provisionado](..\api\channel-provisionemail.md) para um [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="96ff9-105">Represents the email address [provisioned](..\api\channel-provisionemail.md) for a [channel](channel.md).</span></span>

## <a name="properties"></a><span data-ttu-id="96ff9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96ff9-106">Properties</span></span>
| <span data-ttu-id="96ff9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96ff9-107">Property</span></span> | <span data-ttu-id="96ff9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="96ff9-108">Type</span></span>   | <span data-ttu-id="96ff9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="96ff9-109">Description</span></span>                               |
| :------- | :----- | :---------------------------------------- |
| <span data-ttu-id="96ff9-110">email</span><span class="sxs-lookup"><span data-stu-id="96ff9-110">email</span></span>    | <span data-ttu-id="96ff9-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96ff9-111">String</span></span> | <span data-ttu-id="96ff9-112">Representa o endereço de email provisionado.</span><span class="sxs-lookup"><span data-stu-id="96ff9-112">Represents the provisioned email address.</span></span> |

## <a name="relationships"></a><span data-ttu-id="96ff9-113">Relações</span><span class="sxs-lookup"><span data-stu-id="96ff9-113">Relationships</span></span>
<span data-ttu-id="96ff9-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96ff9-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96ff9-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96ff9-115">JSON representation</span></span>
<span data-ttu-id="96ff9-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96ff9-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.provisionChannelEmailResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.provisionChannelEmailResult",
  "email": "String"
}
```
