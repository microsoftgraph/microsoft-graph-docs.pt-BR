---
title: tipo de recurso de audioRoutingGroup
description: O grupo de roteamento áudio armazena uma rota de áudio privada entre os participantes em uma conversa com vários participantes. Fonte é o participante propriamente dito e os receptores são um subconjunto dos outros participantes da conversa com vários participantes.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: cb1b8b67404ef6a3c8f397a6b5debe9acc252b5f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860645"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="e1817-104">tipo de recurso de audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="e1817-104">audioRoutingGroup resource type</span></span>

> <span data-ttu-id="e1817-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1817-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1817-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1817-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1817-107">O grupo de roteamento áudio armazena uma rota de áudio privada entre os participantes em uma conversa com vários participantes.</span><span class="sxs-lookup"><span data-stu-id="e1817-107">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="e1817-108">Fonte é o participante propriamente dito e os receptores são um subconjunto dos outros participantes da conversa com vários participantes.</span><span class="sxs-lookup"><span data-stu-id="e1817-108">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="e1817-109">**Observação:** [ConfigureMixer](../api/participant-configuremixer.md) não envolvem quaisquer rotas, é para toda a chamada para definir os níveis de volume para combinações de receptor de origem.</span><span class="sxs-lookup"><span data-stu-id="e1817-109">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="e1817-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="e1817-110">Methods</span></span>

| <span data-ttu-id="e1817-111">Método</span><span class="sxs-lookup"><span data-stu-id="e1817-111">Method</span></span>                                                  | <span data-ttu-id="e1817-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e1817-112">Return Type</span></span>                               | <span data-ttu-id="e1817-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1817-113">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="e1817-114">Obter audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="e1817-114">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="e1817-115">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="e1817-115">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="e1817-116">Leia as propriedades e os relacionamentos do objeto audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="e1817-116">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="e1817-117">Update</span><span class="sxs-lookup"><span data-stu-id="e1817-117">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="e1817-118">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="e1817-118">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="e1817-119">Lista de receptores de atualização.</span><span class="sxs-lookup"><span data-stu-id="e1817-119">Update receivers list.</span></span>                       |
| [<span data-ttu-id="e1817-120">Delete</span><span class="sxs-lookup"><span data-stu-id="e1817-120">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="e1817-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1817-121">None</span></span>                                      | <span data-ttu-id="e1817-122">Exclua o grupo de roteamento de áudio.</span><span class="sxs-lookup"><span data-stu-id="e1817-122">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="e1817-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1817-123">Properties</span></span>

| <span data-ttu-id="e1817-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1817-124">Property</span></span>      | <span data-ttu-id="e1817-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1817-125">Type</span></span>              | <span data-ttu-id="e1817-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1817-126">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="e1817-127">id</span><span class="sxs-lookup"><span data-stu-id="e1817-127">id</span></span>            | <span data-ttu-id="e1817-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1817-128">String</span></span>            | <span data-ttu-id="e1817-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1817-129">Read-only.</span></span> <span data-ttu-id="e1817-130">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="e1817-130">Server generated.</span></span>                                         |
| <span data-ttu-id="e1817-131">receptores</span><span class="sxs-lookup"><span data-stu-id="e1817-131">receivers</span></span>     | <span data-ttu-id="e1817-132">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1817-132">String Collection</span></span> | <span data-ttu-id="e1817-133">Lista de recebimento de ids de participante.</span><span class="sxs-lookup"><span data-stu-id="e1817-133">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="e1817-134">routingMode</span><span class="sxs-lookup"><span data-stu-id="e1817-134">routingMode</span></span>   | <span data-ttu-id="e1817-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1817-135">String</span></span>            | <span data-ttu-id="e1817-136">Modo de grupo de roteamento.</span><span class="sxs-lookup"><span data-stu-id="e1817-136">Routing group mode.</span></span>  <span data-ttu-id="e1817-137">Os valores possíveis são: `oneToOne` e `multicast`.</span><span class="sxs-lookup"><span data-stu-id="e1817-137">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="e1817-138">sources</span><span class="sxs-lookup"><span data-stu-id="e1817-138">sources</span></span>       | <span data-ttu-id="e1817-139">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1817-139">String Collection</span></span> | <span data-ttu-id="e1817-140">Lista de ids de participante de origem.</span><span class="sxs-lookup"><span data-stu-id="e1817-140">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="e1817-141">**Observação:** Modo de roteamento determina as restrições nas fontes e receptores.</span><span class="sxs-lookup"><span data-stu-id="e1817-141">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="e1817-142">Há suporte para os seguintes grupos de roteamento.</span><span class="sxs-lookup"><span data-stu-id="e1817-142">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="e1817-143">`oneToOne`-fontes e receptores possuem apenas um participante.</span><span class="sxs-lookup"><span data-stu-id="e1817-143">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="e1817-144">`multicast`-fonte com um participante, mas há vários receptores.</span><span class="sxs-lookup"><span data-stu-id="e1817-144">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="e1817-145">Lista de receptores pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="e1817-145">Receivers list may be updated.</span></span>

> <span data-ttu-id="e1817-146">**Observação:** Se você criar vários grupos de roteamento áudio (por exemplo, um bot de cada participante), somente o áudio de superior 4 dominantes alto-falantes será encaminhado.</span><span class="sxs-lookup"><span data-stu-id="e1817-146">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="e1817-147">Isso significa que mesmo com o grupo de roteamento personalizados áudio, se o alto-falante não está alto o suficiente no Misturador de principal, ele/ela não possa ser ouvido pelo bot, mesmo se não houver um grupo de áudio privado apenas para este alto-falante e o bot.</span><span class="sxs-lookup"><span data-stu-id="e1817-147">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="e1817-148">Relações</span><span class="sxs-lookup"><span data-stu-id="e1817-148">Relationships</span></span>
<span data-ttu-id="e1817-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1817-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1817-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1817-150">JSON representation</span></span>

<span data-ttu-id="e1817-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1817-151">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
