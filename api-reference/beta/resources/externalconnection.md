---
title: Tipo de recurso externalConnection
description: Uma conexão é um contêiner lógico para seu conteúdo externo no Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4355ffe51fe1b160c7fb486272e85f2b2cf0bf2c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161696"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="0ce44-103">Tipo de recurso externalConnection</span><span class="sxs-lookup"><span data-stu-id="0ce44-103">externalConnection resource type</span></span>

<span data-ttu-id="0ce44-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ce44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ce44-105">Um contêiner lógico para adicionar conteúdo de uma fonte externa ao Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0ce44-105">A logical container to add content from an external source into Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="0ce44-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0ce44-106">Methods</span></span>

| <span data-ttu-id="0ce44-107">Método</span><span class="sxs-lookup"><span data-stu-id="0ce44-107">Method</span></span>                                                           | <span data-ttu-id="0ce44-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0ce44-108">Return Type</span></span>                                   | <span data-ttu-id="0ce44-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ce44-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="0ce44-110">Criar externalConnection</span><span class="sxs-lookup"><span data-stu-id="0ce44-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="0ce44-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="0ce44-111">externalConnection</span></span>                            | <span data-ttu-id="0ce44-112">Crie uma nova externalConnection postando na coleção connections.</span><span class="sxs-lookup"><span data-stu-id="0ce44-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="0ce44-113">Listar externalConnections</span><span class="sxs-lookup"><span data-stu-id="0ce44-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="0ce44-114">Coleção externalConnection</span><span class="sxs-lookup"><span data-stu-id="0ce44-114">externalConnection collection</span></span>                 | <span data-ttu-id="0ce44-115">Obter uma coleção de objetos externalConnection.</span><span class="sxs-lookup"><span data-stu-id="0ce44-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="0ce44-116">Obter externalConnection</span><span class="sxs-lookup"><span data-stu-id="0ce44-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="0ce44-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="0ce44-117">externalConnection</span></span>                            | <span data-ttu-id="0ce44-118">Leia as propriedades e as relações de um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="0ce44-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="0ce44-119">Atualizar externalConnection</span><span class="sxs-lookup"><span data-stu-id="0ce44-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="0ce44-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="0ce44-120">externalConnection</span></span>                            | <span data-ttu-id="0ce44-121">Atualize um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="0ce44-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="0ce44-122">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="0ce44-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="0ce44-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="0ce44-123">None</span></span>                                          | <span data-ttu-id="0ce44-124">Exclua um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="0ce44-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="0ce44-125">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="0ce44-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="0ce44-126">Nenhum *ou* [esquema](schema.md)</span><span class="sxs-lookup"><span data-stu-id="0ce44-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="0ce44-127">Registre o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="0ce44-127">Register connection schema.</span></span> |
| [<span data-ttu-id="0ce44-128">Obter operação</span><span class="sxs-lookup"><span data-stu-id="0ce44-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="0ce44-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="0ce44-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="0ce44-130">Obter o status de uma solicitação assíncrona para criar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="0ce44-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="0ce44-131">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="0ce44-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="0ce44-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="0ce44-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="0ce44-133">Crie um novo externalItem postando na coleção de itens.</span><span class="sxs-lookup"><span data-stu-id="0ce44-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="0ce44-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ce44-134">Properties</span></span>

| <span data-ttu-id="0ce44-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ce44-135">Property</span></span>      | <span data-ttu-id="0ce44-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ce44-136">Type</span></span>                              | <span data-ttu-id="0ce44-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ce44-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="0ce44-138">configuração</span><span class="sxs-lookup"><span data-stu-id="0ce44-138">configuration</span></span> | [<span data-ttu-id="0ce44-139">configuration</span><span class="sxs-lookup"><span data-stu-id="0ce44-139">configuration</span></span>](configuration.md) | <span data-ttu-id="0ce44-140">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar conteúdo na conexão.</span><span class="sxs-lookup"><span data-stu-id="0ce44-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="0ce44-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0ce44-141">Optional.</span></span> |
| <span data-ttu-id="0ce44-142">description</span><span class="sxs-lookup"><span data-stu-id="0ce44-142">description</span></span>   | <span data-ttu-id="0ce44-143">String</span><span class="sxs-lookup"><span data-stu-id="0ce44-143">String</span></span>                            | <span data-ttu-id="0ce44-144">Descrição da conexão exibida no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0ce44-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="0ce44-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0ce44-145">Optional.</span></span> |
| <span data-ttu-id="0ce44-146">id</span><span class="sxs-lookup"><span data-stu-id="0ce44-146">id</span></span>            | <span data-ttu-id="0ce44-147">String</span><span class="sxs-lookup"><span data-stu-id="0ce44-147">String</span></span>                            | <span data-ttu-id="0ce44-148">ID exclusiva fornecida pelo desenvolvedor da conexão no locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0ce44-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="0ce44-149">Comprimento máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="0ce44-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="0ce44-150">Deve conter apenas caracteres alfanuméricos.</span><span class="sxs-lookup"><span data-stu-id="0ce44-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="0ce44-151">Não pode começar `Microsoft` com ou ser um dos seguintes valores: , , `None` , , , , , , `Directory` , `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` , `Connectors`</span><span class="sxs-lookup"><span data-stu-id="0ce44-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="0ce44-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ce44-152">Required.</span></span> |
| <span data-ttu-id="0ce44-153">name</span><span class="sxs-lookup"><span data-stu-id="0ce44-153">name</span></span>          | <span data-ttu-id="0ce44-154">String</span><span class="sxs-lookup"><span data-stu-id="0ce44-154">String</span></span>                            | <span data-ttu-id="0ce44-155">O nome de exibição da conexão a ser exibida no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0ce44-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="0ce44-156">Comprimento máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="0ce44-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="0ce44-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ce44-157">Required.</span></span> |
| <span data-ttu-id="0ce44-158">estado</span><span class="sxs-lookup"><span data-stu-id="0ce44-158">state</span></span>         | <span data-ttu-id="0ce44-159">connectionState</span><span class="sxs-lookup"><span data-stu-id="0ce44-159">connectionState</span></span>                   | <span data-ttu-id="0ce44-160">Indica o estado atual da conexão.</span><span class="sxs-lookup"><span data-stu-id="0ce44-160">Indicates the current state of the connection.</span></span> <span data-ttu-id="0ce44-161">Os valores possíveis `draft` `ready` são , e `obsolete` `limitExceeded` .</span><span class="sxs-lookup"><span data-stu-id="0ce44-161">Possible values are `draft`, `ready`, `obsolete`, and `limitExceeded`.</span></span> <span data-ttu-id="0ce44-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ce44-162">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0ce44-163">Relações</span><span class="sxs-lookup"><span data-stu-id="0ce44-163">Relationships</span></span>

| <span data-ttu-id="0ce44-164">Relação</span><span class="sxs-lookup"><span data-stu-id="0ce44-164">Relationship</span></span> | <span data-ttu-id="0ce44-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ce44-165">Type</span></span>                                                     | <span data-ttu-id="0ce44-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ce44-166">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="0ce44-167">items</span><span class="sxs-lookup"><span data-stu-id="0ce44-167">items</span></span>        | <span data-ttu-id="0ce44-168">[Coleção externalItem](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ce44-168">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="0ce44-p106">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0ce44-p106">Read-only. Nullable.</span></span> |
| <span data-ttu-id="0ce44-171">operations</span><span class="sxs-lookup"><span data-stu-id="0ce44-171">operations</span></span>   | <span data-ttu-id="0ce44-172">[Coleção connectionOperation](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0ce44-172">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="0ce44-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ce44-173">Read-only.</span></span> <span data-ttu-id="0ce44-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="0ce44-174">Nullable.</span></span> |
| <span data-ttu-id="0ce44-175">esquema</span><span class="sxs-lookup"><span data-stu-id="0ce44-175">schema</span></span>       | [<span data-ttu-id="0ce44-176">schema</span><span class="sxs-lookup"><span data-stu-id="0ce44-176">schema</span></span>](schema.md)                                      | <span data-ttu-id="0ce44-p108">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0ce44-p108">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ce44-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ce44-179">JSON representation</span></span>

<span data-ttu-id="0ce44-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ce44-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "keyProperty": "id"
}-->

```json
{
  "configuration": {"@odata.type": "microsoft.graph.configuration"},
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
