---
title: tipo de recurso de audioRoutingGroup
description: O grupo de roteamento áudio armazena uma rota de áudio privada entre os participantes em uma conversa com vários participantes. Fonte é o participante propriamente dito e os receptores são um subconjunto dos outros participantes da conversa com vários participantes.
ms.openlocfilehash: 98c58e39773567f13a2723e94c0413efd2841cd0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033496"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="35c08-104">tipo de recurso de audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="35c08-104">audioRoutingGroup resource type</span></span>

> <span data-ttu-id="35c08-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="35c08-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35c08-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="35c08-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35c08-107">O grupo de roteamento áudio armazena uma rota de áudio privada entre os participantes em uma conversa com vários participantes.</span><span class="sxs-lookup"><span data-stu-id="35c08-107">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="35c08-108">Fonte é o participante propriamente dito e os receptores são um subconjunto dos outros participantes da conversa com vários participantes.</span><span class="sxs-lookup"><span data-stu-id="35c08-108">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="35c08-109">**Observação:** [ConfigureMixer](../api/participant-configuremixer.md) não envolvem quaisquer rotas, é para toda a chamada para definir os níveis de volume para combinações de receptor de origem.</span><span class="sxs-lookup"><span data-stu-id="35c08-109">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="35c08-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="35c08-110">Methods</span></span>

| <span data-ttu-id="35c08-111">Método</span><span class="sxs-lookup"><span data-stu-id="35c08-111">Method</span></span>                                                  | <span data-ttu-id="35c08-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="35c08-112">Return Type</span></span>                               | <span data-ttu-id="35c08-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="35c08-113">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="35c08-114">Obter audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="35c08-114">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="35c08-115">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="35c08-115">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="35c08-116">Leia as propriedades e os relacionamentos do objeto audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="35c08-116">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="35c08-117">Update</span><span class="sxs-lookup"><span data-stu-id="35c08-117">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="35c08-118">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="35c08-118">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="35c08-119">Lista de receptores de atualização.</span><span class="sxs-lookup"><span data-stu-id="35c08-119">Update receivers list.</span></span>                       |
| [<span data-ttu-id="35c08-120">Delete</span><span class="sxs-lookup"><span data-stu-id="35c08-120">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="35c08-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35c08-121">None</span></span>                                      | <span data-ttu-id="35c08-122">Exclua o grupo de roteamento de áudio.</span><span class="sxs-lookup"><span data-stu-id="35c08-122">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="35c08-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35c08-123">Properties</span></span>

| <span data-ttu-id="35c08-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35c08-124">Property</span></span>      | <span data-ttu-id="35c08-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="35c08-125">Type</span></span>              | <span data-ttu-id="35c08-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="35c08-126">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="35c08-127">id</span><span class="sxs-lookup"><span data-stu-id="35c08-127">id</span></span>            | <span data-ttu-id="35c08-128">String</span><span class="sxs-lookup"><span data-stu-id="35c08-128">String</span></span>            | <span data-ttu-id="35c08-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35c08-129">Read-only.</span></span> <span data-ttu-id="35c08-130">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="35c08-130">Server generated.</span></span>                                         |
| <span data-ttu-id="35c08-131">receptores</span><span class="sxs-lookup"><span data-stu-id="35c08-131">receivers</span></span>     | <span data-ttu-id="35c08-132">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35c08-132">String Collection</span></span> | <span data-ttu-id="35c08-133">Lista de recebimento de ids de participante.</span><span class="sxs-lookup"><span data-stu-id="35c08-133">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="35c08-134">routingMode</span><span class="sxs-lookup"><span data-stu-id="35c08-134">routingMode</span></span>   | <span data-ttu-id="35c08-135">String</span><span class="sxs-lookup"><span data-stu-id="35c08-135">String</span></span>            | <span data-ttu-id="35c08-136">Modo de grupo de roteamento.</span><span class="sxs-lookup"><span data-stu-id="35c08-136">Routing group mode.</span></span>  <span data-ttu-id="35c08-137">Os valores possíveis são: `oneToOne` e `multicast`.</span><span class="sxs-lookup"><span data-stu-id="35c08-137">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="35c08-138">sources</span><span class="sxs-lookup"><span data-stu-id="35c08-138">sources</span></span>       | <span data-ttu-id="35c08-139">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35c08-139">String Collection</span></span> | <span data-ttu-id="35c08-140">Lista de ids de participante de origem.</span><span class="sxs-lookup"><span data-stu-id="35c08-140">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="35c08-141">**Observação:** Modo de roteamento determina as restrições nas fontes e receptores.</span><span class="sxs-lookup"><span data-stu-id="35c08-141">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="35c08-142">Há suporte para os seguintes grupos de roteamento.</span><span class="sxs-lookup"><span data-stu-id="35c08-142">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="35c08-143">`oneToOne`-fontes e receptores possuem apenas um participante.</span><span class="sxs-lookup"><span data-stu-id="35c08-143">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="35c08-144">`multicast`-fonte com um participante, mas há vários receptores.</span><span class="sxs-lookup"><span data-stu-id="35c08-144">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="35c08-145">Lista de receptores pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="35c08-145">Receivers list may be updated.</span></span>

> <span data-ttu-id="35c08-146">**Observação:** Se você criar vários grupos de roteamento áudio (por exemplo, um bot de cada participante), somente o áudio de superior 4 dominantes alto-falantes será encaminhado.</span><span class="sxs-lookup"><span data-stu-id="35c08-146">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="35c08-147">Isso significa que mesmo com o grupo de roteamento personalizados áudio, se o alto-falante não está alto o suficiente no Misturador de principal, ele/ela não possa ser ouvido pelo bot, mesmo se não houver um grupo de áudio privado apenas para este alto-falante e o bot.</span><span class="sxs-lookup"><span data-stu-id="35c08-147">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="35c08-148">Relações</span><span class="sxs-lookup"><span data-stu-id="35c08-148">Relationships</span></span>
<span data-ttu-id="35c08-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35c08-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35c08-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35c08-150">JSON representation</span></span>

<span data-ttu-id="35c08-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35c08-151">The following is a JSON representation of the resource.</span></span>

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
