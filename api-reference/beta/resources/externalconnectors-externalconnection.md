---
title: Tipo de recurso externalConnection
description: Uma conexão é um contêiner lógico para seu conteúdo externo no Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 76fa391d1ce9937bc1799e9bc4ae9470c0794497
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467569"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="2c783-103">Tipo de recurso externalConnection</span><span class="sxs-lookup"><span data-stu-id="2c783-103">externalConnection resource type</span></span>

<span data-ttu-id="2c783-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="2c783-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c783-105">Um contêiner lógico para adicionar conteúdo de uma fonte externa à Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2c783-105">A logical container to add content from an external source into Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="2c783-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2c783-106">Methods</span></span>

| <span data-ttu-id="2c783-107">Método</span><span class="sxs-lookup"><span data-stu-id="2c783-107">Method</span></span>                                                           | <span data-ttu-id="2c783-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2c783-108">Return Type</span></span>                                   | <span data-ttu-id="2c783-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c783-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="2c783-110">Criar externalConnection</span><span class="sxs-lookup"><span data-stu-id="2c783-110">Create externalConnection</span></span>](../api/externalconnectors-external-post-connections.md) | <span data-ttu-id="2c783-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="2c783-111">externalConnection</span></span>                            | <span data-ttu-id="2c783-112">Crie um novo externalConnection postando na coleção connections.</span><span class="sxs-lookup"><span data-stu-id="2c783-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="2c783-113">Listar externalConnections</span><span class="sxs-lookup"><span data-stu-id="2c783-113">List externalConnections</span></span>](../api/externalconnectors-externalconnection-list.md)    | <span data-ttu-id="2c783-114">Coleção externalConnection</span><span class="sxs-lookup"><span data-stu-id="2c783-114">externalConnection collection</span></span>                 | <span data-ttu-id="2c783-115">Obter uma coleção de objetos externalConnection.</span><span class="sxs-lookup"><span data-stu-id="2c783-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="2c783-116">Obter externalConnection</span><span class="sxs-lookup"><span data-stu-id="2c783-116">Get externalConnection</span></span>](../api/externalconnectors-externalconnection-get.md)       | <span data-ttu-id="2c783-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="2c783-117">externalConnection</span></span>                            | <span data-ttu-id="2c783-118">Ler propriedades e relações de um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="2c783-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="2c783-119">Atualizar externalConnection</span><span class="sxs-lookup"><span data-stu-id="2c783-119">Update externalConnection</span></span>](../api/externalconnectors-externalconnection-update.md) | <span data-ttu-id="2c783-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="2c783-120">externalConnection</span></span>                            | <span data-ttu-id="2c783-121">Atualize um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="2c783-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="2c783-122">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="2c783-122">Delete externalConnection</span></span>](../api/externalconnectors-externalconnection-delete.md) | <span data-ttu-id="2c783-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c783-123">None</span></span>                                          | <span data-ttu-id="2c783-124">Exclua um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="2c783-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="2c783-125">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="2c783-125">Create schema</span></span>](../api/externalconnectors-externalconnection-post-schema.md)        | <span data-ttu-id="2c783-126">Nenhum *ou* [esquema](externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="2c783-126">None *or* [schema](externalconnectors-schema.md)</span></span>                 | <span data-ttu-id="2c783-127">Registrar esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="2c783-127">Register connection schema.</span></span> |
| [<span data-ttu-id="2c783-128">Obter operação</span><span class="sxs-lookup"><span data-stu-id="2c783-128">Get operation</span></span>](../api/externalconnectors-connectionoperation-get.md)               | [<span data-ttu-id="2c783-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="2c783-129">connectionOperation</span></span>](externalconnectors-connectionoperation.md) | <span data-ttu-id="2c783-130">Obter o status de uma solicitação assíncrona para criar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="2c783-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="2c783-131">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="2c783-131">Create externalItem</span></span>](../api/externalconnectors-externalconnection-put-items.md)    | [<span data-ttu-id="2c783-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="2c783-132">externalItem</span></span>](externalconnectors-externalitem.md)               | <span data-ttu-id="2c783-133">Crie um novo externalItem postando na coleção items.</span><span class="sxs-lookup"><span data-stu-id="2c783-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="2c783-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c783-134">Properties</span></span>

| <span data-ttu-id="2c783-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c783-135">Property</span></span>      | <span data-ttu-id="2c783-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c783-136">Type</span></span>                              | <span data-ttu-id="2c783-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c783-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="2c783-138">configuração</span><span class="sxs-lookup"><span data-stu-id="2c783-138">configuration</span></span> | [<span data-ttu-id="2c783-139">microsoft.graph.externalConnectors.configuration</span><span class="sxs-lookup"><span data-stu-id="2c783-139">microsoft.graph.externalConnectors.configuration</span></span>](externalconnectors-configuration.md) | <span data-ttu-id="2c783-140">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar conteúdo na conexão.</span><span class="sxs-lookup"><span data-stu-id="2c783-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="2c783-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2c783-141">Optional.</span></span> |
| <span data-ttu-id="2c783-142">description</span><span class="sxs-lookup"><span data-stu-id="2c783-142">description</span></span>   | <span data-ttu-id="2c783-143">String</span><span class="sxs-lookup"><span data-stu-id="2c783-143">String</span></span>                            | <span data-ttu-id="2c783-144">Descrição da conexão exibida no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2c783-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="2c783-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2c783-145">Optional.</span></span> |
| <span data-ttu-id="2c783-146">id</span><span class="sxs-lookup"><span data-stu-id="2c783-146">id</span></span>            | <span data-ttu-id="2c783-147">String</span><span class="sxs-lookup"><span data-stu-id="2c783-147">String</span></span>                            | <span data-ttu-id="2c783-148">ID exclusiva fornecida pelo desenvolvedor da conexão no Azure Active Directory locatário.</span><span class="sxs-lookup"><span data-stu-id="2c783-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="2c783-149">Deve ter entre 3 e 32 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="2c783-149">Must be between 3 and 32 characters in length.</span></span> <span data-ttu-id="2c783-150">Deve conter somente caracteres alfanuméricos.</span><span class="sxs-lookup"><span data-stu-id="2c783-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="2c783-151">Não é possível começar ou ser um dos `Microsoft` seguintes valores: `None` , , , , , , , , `Directory` , , , , `Exchange` , , `ExchangeArchive` , `LinkedIn` , `Mailbox` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` `TaskFabric` `PowerBI` `Assistant` `TopicEngine` . `MSFT_All_Connectors`</span><span class="sxs-lookup"><span data-stu-id="2c783-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`, `TaskFabric`, `PowerBI`, `Assistant`, `TopicEngine`, `MSFT_All_Connectors`.</span></span> <span data-ttu-id="2c783-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c783-152">Required.</span></span> |
| <span data-ttu-id="2c783-153">nome</span><span class="sxs-lookup"><span data-stu-id="2c783-153">name</span></span>          | <span data-ttu-id="2c783-154">String</span><span class="sxs-lookup"><span data-stu-id="2c783-154">String</span></span>                            | <span data-ttu-id="2c783-155">O nome de exibição da conexão a ser exibida no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2c783-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="2c783-156">Comprimento máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="2c783-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="2c783-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c783-157">Required.</span></span> |
| <span data-ttu-id="2c783-158">state</span><span class="sxs-lookup"><span data-stu-id="2c783-158">state</span></span>         | <span data-ttu-id="2c783-159">microsoft.graph.externalConnectors.connectionState</span><span class="sxs-lookup"><span data-stu-id="2c783-159">microsoft.graph.externalConnectors.connectionState</span></span>                   | <span data-ttu-id="2c783-160">Indica o estado atual da conexão.</span><span class="sxs-lookup"><span data-stu-id="2c783-160">Indicates the current state of the connection.</span></span> <span data-ttu-id="2c783-161">Os valores possíveis `draft` `ready` são , e `obsolete` `limitExceeded` .</span><span class="sxs-lookup"><span data-stu-id="2c783-161">Possible values are `draft`, `ready`, `obsolete`, and `limitExceeded`.</span></span> <span data-ttu-id="2c783-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c783-162">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2c783-163">Relações</span><span class="sxs-lookup"><span data-stu-id="2c783-163">Relationships</span></span>

| <span data-ttu-id="2c783-164">Relação</span><span class="sxs-lookup"><span data-stu-id="2c783-164">Relationship</span></span> | <span data-ttu-id="2c783-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c783-165">Type</span></span>                                                     | <span data-ttu-id="2c783-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c783-166">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="2c783-167">items</span><span class="sxs-lookup"><span data-stu-id="2c783-167">items</span></span>        | <span data-ttu-id="2c783-168">[Coleção microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="2c783-168">[microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md) collection</span></span>               | <span data-ttu-id="2c783-p106">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2c783-p106">Read-only. Nullable.</span></span> |
| <span data-ttu-id="2c783-171">operations</span><span class="sxs-lookup"><span data-stu-id="2c783-171">operations</span></span>   | <span data-ttu-id="2c783-172">[coleção microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="2c783-172">[microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md) collection</span></span> | <span data-ttu-id="2c783-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2c783-p107">Read-only. Nullable.</span></span> |
| <span data-ttu-id="2c783-175">schema</span><span class="sxs-lookup"><span data-stu-id="2c783-175">schema</span></span>       | [<span data-ttu-id="2c783-176">microsoft.graph.externalConnectors.schema</span><span class="sxs-lookup"><span data-stu-id="2c783-176">microsoft.graph.externalConnectors.schema</span></span>](externalconnectors-schema.md)                                      | <span data-ttu-id="2c783-p108">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2c783-p108">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2c783-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c783-179">JSON representation</span></span>

<span data-ttu-id="2c783-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c783-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "name": "String",
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
