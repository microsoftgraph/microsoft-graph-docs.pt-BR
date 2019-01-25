---
title: tipo de recurso de audioRoutingGroup
description: O grupo de roteamento áudio armazena uma rota de áudio privada entre os participantes em uma conversa com vários participantes. Fonte é o participante propriamente dito e os receptores são um subconjunto dos outros participantes da conversa com vários participantes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e7fc7de5b5caaa2f4079c453f9cd855a42577cb8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509620"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="d0bf2-104">tipo de recurso de audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="d0bf2-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0bf2-105">O grupo de roteamento áudio armazena uma rota de áudio privada entre os participantes em uma conversa com vários participantes.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="d0bf2-106">Fonte é o participante propriamente dito e os receptores são um subconjunto dos outros participantes da conversa com vários participantes.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="d0bf2-107">**Observação:** [ConfigureMixer](../api/participant-configuremixer.md) não envolvem quaisquer rotas, é para toda a chamada para definir os níveis de volume para combinações de receptor de origem.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="d0bf2-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d0bf2-108">Methods</span></span>

| <span data-ttu-id="d0bf2-109">Método</span><span class="sxs-lookup"><span data-stu-id="d0bf2-109">Method</span></span>                                                  | <span data-ttu-id="d0bf2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d0bf2-110">Return Type</span></span>                               | <span data-ttu-id="d0bf2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0bf2-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="d0bf2-112">Obter audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="d0bf2-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="d0bf2-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="d0bf2-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="d0bf2-114">Leia as propriedades e os relacionamentos do objeto audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="d0bf2-115">Update</span><span class="sxs-lookup"><span data-stu-id="d0bf2-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="d0bf2-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="d0bf2-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="d0bf2-117">Lista de receptores de atualização.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="d0bf2-118">Delete</span><span class="sxs-lookup"><span data-stu-id="d0bf2-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="d0bf2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d0bf2-119">None</span></span>                                      | <span data-ttu-id="d0bf2-120">Exclua o grupo de roteamento de áudio.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="d0bf2-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0bf2-121">Properties</span></span>

| <span data-ttu-id="d0bf2-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0bf2-122">Property</span></span>      | <span data-ttu-id="d0bf2-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0bf2-123">Type</span></span>              | <span data-ttu-id="d0bf2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0bf2-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="d0bf2-125">id</span><span class="sxs-lookup"><span data-stu-id="d0bf2-125">id</span></span>            | <span data-ttu-id="d0bf2-126">String</span><span class="sxs-lookup"><span data-stu-id="d0bf2-126">String</span></span>            | <span data-ttu-id="d0bf2-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-127">Read-only.</span></span> <span data-ttu-id="d0bf2-128">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-128">Server generated.</span></span>                                         |
| <span data-ttu-id="d0bf2-129">receptores</span><span class="sxs-lookup"><span data-stu-id="d0bf2-129">receivers</span></span>     | <span data-ttu-id="d0bf2-130">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0bf2-130">String Collection</span></span> | <span data-ttu-id="d0bf2-131">Lista de recebimento de ids de participante.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="d0bf2-132">routingMode</span><span class="sxs-lookup"><span data-stu-id="d0bf2-132">routingMode</span></span>   | <span data-ttu-id="d0bf2-133">String</span><span class="sxs-lookup"><span data-stu-id="d0bf2-133">String</span></span>            | <span data-ttu-id="d0bf2-134">Modo de grupo de roteamento.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-134">Routing group mode.</span></span>  <span data-ttu-id="d0bf2-135">Os valores possíveis são: `oneToOne` e `multicast`.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="d0bf2-136">sources</span><span class="sxs-lookup"><span data-stu-id="d0bf2-136">sources</span></span>       | <span data-ttu-id="d0bf2-137">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0bf2-137">String Collection</span></span> | <span data-ttu-id="d0bf2-138">Lista de ids de participante de origem.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="d0bf2-139">**Observação:** Modo de roteamento determina as restrições nas fontes e receptores.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="d0bf2-140">Há suporte para os seguintes grupos de roteamento.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="d0bf2-141">`oneToOne`-fontes e receptores possuem apenas um participante.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="d0bf2-142">`multicast`-fonte com um participante, mas há vários receptores.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="d0bf2-143">Lista de receptores pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="d0bf2-144">**Observação:** Se você criar vários grupos de roteamento áudio (por exemplo, um bot de cada participante), somente o áudio de superior 4 dominantes alto-falantes será encaminhado.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="d0bf2-145">Isso significa que mesmo com o grupo de roteamento personalizados áudio, se o alto-falante não está alto o suficiente no Misturador de principal, ele/ela não possa ser ouvido pelo bot, mesmo se não houver um grupo de áudio privado apenas para este alto-falante e o bot.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="d0bf2-146">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="d0bf2-146">Relationships</span></span>
<span data-ttu-id="d0bf2-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d0bf2-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0bf2-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0bf2-148">JSON representation</span></span>

<span data-ttu-id="d0bf2-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0bf2-149">The following is a JSON representation of the resource.</span></span>

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
