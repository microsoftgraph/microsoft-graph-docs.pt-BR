---
title: tipo de recurso audioRoutingGroup
description: O grupo de roteamento de áudio armazena uma rota de áudio privada entre os participantes de uma conversa de várias partes. Source é o próprio participante e os receptores são um subconjunto de outros participantes da conversa de vários participantes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e7fc7de5b5caaa2f4079c453f9cd855a42577cb8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543998"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="b1a8f-104">tipo de recurso audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b1a8f-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1a8f-105">O grupo de roteamento de áudio armazena uma rota de áudio privada entre os participantes de uma conversa de várias partes.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="b1a8f-106">Source é o próprio participante e os receptores são um subconjunto de outros participantes da conversa de vários participantes.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="b1a8f-107">**Observação:** O [ConfigureMixer](../api/participant-configuremixer.md) não envolve nenhuma rota, é para toda a chamada para definir os níveis de volume para combinações de receptor de origem.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="b1a8f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b1a8f-108">Methods</span></span>

| <span data-ttu-id="b1a8f-109">Método</span><span class="sxs-lookup"><span data-stu-id="b1a8f-109">Method</span></span>                                                  | <span data-ttu-id="b1a8f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b1a8f-110">Return Type</span></span>                               | <span data-ttu-id="b1a8f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1a8f-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="b1a8f-112">Obter audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b1a8f-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="b1a8f-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b1a8f-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="b1a8f-114">Leia as propriedades e os relacionamentos do objeto audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="b1a8f-115">Update</span><span class="sxs-lookup"><span data-stu-id="b1a8f-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="b1a8f-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b1a8f-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="b1a8f-117">Atualizar lista de receptores.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="b1a8f-118">Excluir</span><span class="sxs-lookup"><span data-stu-id="b1a8f-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="b1a8f-119">None</span><span class="sxs-lookup"><span data-stu-id="b1a8f-119">None</span></span>                                      | <span data-ttu-id="b1a8f-120">Exclua o grupo roteamento de áudio.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="b1a8f-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1a8f-121">Properties</span></span>

| <span data-ttu-id="b1a8f-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1a8f-122">Property</span></span>      | <span data-ttu-id="b1a8f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1a8f-123">Type</span></span>              | <span data-ttu-id="b1a8f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1a8f-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="b1a8f-125">id</span><span class="sxs-lookup"><span data-stu-id="b1a8f-125">id</span></span>            | <span data-ttu-id="b1a8f-126">String</span><span class="sxs-lookup"><span data-stu-id="b1a8f-126">String</span></span>            | <span data-ttu-id="b1a8f-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-127">Read-only.</span></span> <span data-ttu-id="b1a8f-128">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-128">Server generated.</span></span>                                         |
| <span data-ttu-id="b1a8f-129">receptores</span><span class="sxs-lookup"><span data-stu-id="b1a8f-129">receivers</span></span>     | <span data-ttu-id="b1a8f-130">String Collection</span><span class="sxs-lookup"><span data-stu-id="b1a8f-130">String Collection</span></span> | <span data-ttu-id="b1a8f-131">Lista de IDs de participantes de recebimento.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="b1a8f-132">routingmode</span><span class="sxs-lookup"><span data-stu-id="b1a8f-132">routingMode</span></span>   | <span data-ttu-id="b1a8f-133">String</span><span class="sxs-lookup"><span data-stu-id="b1a8f-133">String</span></span>            | <span data-ttu-id="b1a8f-134">Modo de grupo de roteamento.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-134">Routing group mode.</span></span>  <span data-ttu-id="b1a8f-135">Os valores possíveis são: `oneToOne` e `multicast`.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="b1a8f-136">fontes</span><span class="sxs-lookup"><span data-stu-id="b1a8f-136">sources</span></span>       | <span data-ttu-id="b1a8f-137">String Collection</span><span class="sxs-lookup"><span data-stu-id="b1a8f-137">String Collection</span></span> | <span data-ttu-id="b1a8f-138">Lista de IDs de participantes de origem.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="b1a8f-139">**Observação:** O modo de roteamento determina as restrições nas fontes e nos receptores.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="b1a8f-140">Só há suporte para os seguintes grupos de roteamento.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="b1a8f-141">`oneToOne`– fontes e receptores têm apenas um participante a cada.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="b1a8f-142">`multicast`-a fonte tem um participante, mas há vários receptores.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="b1a8f-143">A lista de receptores pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="b1a8f-144">**Observação:** Se você criar muitos grupos de roteamento de áudio (por exemplo, um bot por participante), apenas o áudio dos quatro alto-falantes mais dominantes será encaminhado.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="b1a8f-145">Isso significa mesmo com o grupo de roteamento de áudio personalizado, se o alto-falante não estiver suficientemente alto no mixer principal, ele/ela não poderá ser ouvido pelo bot, mesmo se houver um grupo de áudio privado apenas para esse alto-falante e o bot.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="b1a8f-146">Relações</span><span class="sxs-lookup"><span data-stu-id="b1a8f-146">Relationships</span></span>
<span data-ttu-id="b1a8f-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1a8f-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1a8f-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1a8f-148">JSON representation</span></span>

<span data-ttu-id="b1a8f-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1a8f-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "String" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "String" ]
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
  "suppressions": [
    "Error: /api-reference/beta/resources/audioroutinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
