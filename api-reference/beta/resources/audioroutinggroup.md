---
title: tipo de recurso audioRoutingGroup
description: O grupo de roteamento de áudio armazena uma rota de áudio privada entre os participantes de uma conversa de várias partes. Source é o próprio participante e os receptores são um subconjunto de outros participantes da conversa de vários participantes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: db5f94f9ac500dfeb97c6eb787783e9f749ae507
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974273"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="45f92-104">tipo de recurso audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="45f92-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45f92-105">O grupo de roteamento de áudio armazena uma rota de áudio privada entre os participantes de uma conversa de várias partes.</span><span class="sxs-lookup"><span data-stu-id="45f92-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="45f92-106">Source é o próprio participante e os receptores são um subconjunto de outros participantes da conversa de vários participantes.</span><span class="sxs-lookup"><span data-stu-id="45f92-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="45f92-107">**Observação:** O [ConfigureMixer](../api/participant-configuremixer.md) não envolve nenhuma rota, é para toda a chamada para definir os níveis de volume para combinações de receptor de origem.</span><span class="sxs-lookup"><span data-stu-id="45f92-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="45f92-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="45f92-108">Methods</span></span>

| <span data-ttu-id="45f92-109">Método</span><span class="sxs-lookup"><span data-stu-id="45f92-109">Method</span></span>                                                  | <span data-ttu-id="45f92-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="45f92-110">Return Type</span></span>                               | <span data-ttu-id="45f92-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="45f92-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="45f92-112">Obter audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="45f92-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="45f92-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="45f92-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="45f92-114">Leia as propriedades e os relacionamentos do objeto audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="45f92-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="45f92-115">Atualização</span><span class="sxs-lookup"><span data-stu-id="45f92-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="45f92-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="45f92-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="45f92-117">Atualizar lista de receptores.</span><span class="sxs-lookup"><span data-stu-id="45f92-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="45f92-118">Delete</span><span class="sxs-lookup"><span data-stu-id="45f92-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="45f92-119">None</span><span class="sxs-lookup"><span data-stu-id="45f92-119">None</span></span>                                      | <span data-ttu-id="45f92-120">Exclua o grupo roteamento de áudio.</span><span class="sxs-lookup"><span data-stu-id="45f92-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="45f92-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45f92-121">Properties</span></span>

| <span data-ttu-id="45f92-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45f92-122">Property</span></span>      | <span data-ttu-id="45f92-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="45f92-123">Type</span></span>              | <span data-ttu-id="45f92-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="45f92-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="45f92-125">id</span><span class="sxs-lookup"><span data-stu-id="45f92-125">id</span></span>            | <span data-ttu-id="45f92-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45f92-126">string</span></span>            | <span data-ttu-id="45f92-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45f92-127">Read-only.</span></span> <span data-ttu-id="45f92-128">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="45f92-128">Server generated.</span></span>                                         |
| <span data-ttu-id="45f92-129">receptores</span><span class="sxs-lookup"><span data-stu-id="45f92-129">receivers</span></span>     | <span data-ttu-id="45f92-130">collection(string)</span><span class="sxs-lookup"><span data-stu-id="45f92-130">collection(string)</span></span> | <span data-ttu-id="45f92-131">Lista de IDs de participantes de recebimento.</span><span class="sxs-lookup"><span data-stu-id="45f92-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="45f92-132">routingmode</span><span class="sxs-lookup"><span data-stu-id="45f92-132">routingMode</span></span>   | <span data-ttu-id="45f92-133">string</span><span class="sxs-lookup"><span data-stu-id="45f92-133">string</span></span>            | <span data-ttu-id="45f92-134">Modo de grupo de roteamento.</span><span class="sxs-lookup"><span data-stu-id="45f92-134">Routing group mode.</span></span>  <span data-ttu-id="45f92-135">Os valores possíveis são: `oneToOne` e `multicast`.</span><span class="sxs-lookup"><span data-stu-id="45f92-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="45f92-136">fontes</span><span class="sxs-lookup"><span data-stu-id="45f92-136">sources</span></span>       | <span data-ttu-id="45f92-137">collection(string)</span><span class="sxs-lookup"><span data-stu-id="45f92-137">collection(string)</span></span> | <span data-ttu-id="45f92-138">Lista de IDs de participantes de origem.</span><span class="sxs-lookup"><span data-stu-id="45f92-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="45f92-139">**Observação:** O modo de roteamento determina as restrições nas fontes e nos receptores.</span><span class="sxs-lookup"><span data-stu-id="45f92-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="45f92-140">Só há suporte para os seguintes grupos de roteamento.</span><span class="sxs-lookup"><span data-stu-id="45f92-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="45f92-141">`oneToOne`– fontes e receptores têm apenas um participante a cada.</span><span class="sxs-lookup"><span data-stu-id="45f92-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="45f92-142">`multicast`-a fonte tem um participante, mas há vários receptores.</span><span class="sxs-lookup"><span data-stu-id="45f92-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="45f92-143">A lista de receptores pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="45f92-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="45f92-144">**Observação:** Se você criar muitos grupos de roteamento de áudio (por exemplo, um bot por participante), apenas o áudio dos quatro alto-falantes mais dominantes será encaminhado.</span><span class="sxs-lookup"><span data-stu-id="45f92-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="45f92-145">Isso significa mesmo com o grupo de roteamento de áudio personalizado, se o alto-falante não estiver suficientemente alto no mixer principal, ele/ela não poderá ser ouvido pelo bot, mesmo se houver um grupo de áudio privado apenas para esse alto-falante e o bot.</span><span class="sxs-lookup"><span data-stu-id="45f92-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="45f92-146">Relações</span><span class="sxs-lookup"><span data-stu-id="45f92-146">Relationships</span></span>
<span data-ttu-id="45f92-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45f92-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45f92-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45f92-148">JSON representation</span></span>

<span data-ttu-id="45f92-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45f92-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "string (identifier)",
  "receivers": [ "string" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "string" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
