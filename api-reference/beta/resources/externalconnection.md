---
title: tipo de recurso externalConnection
description: Uma conexão com a Microsoft Search a partir de uma fonte externa.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a5db824fabc1cedb27d15c4b2cbfbce08bd59191
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026926"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="a6e81-103">tipo de recurso externalConnection</span><span class="sxs-lookup"><span data-stu-id="a6e81-103">externalConnection resource type</span></span>

<span data-ttu-id="a6e81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6e81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6e81-105">Uma conexão com a Microsoft Search a partir de uma fonte externa.</span><span class="sxs-lookup"><span data-stu-id="a6e81-105">A connection to Microsoft Search from an external source.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="a6e81-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a6e81-106">Methods</span></span>

| <span data-ttu-id="a6e81-107">Método</span><span class="sxs-lookup"><span data-stu-id="a6e81-107">Method</span></span>                                                           | <span data-ttu-id="a6e81-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a6e81-108">Return Type</span></span>                                   | <span data-ttu-id="a6e81-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6e81-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="a6e81-110">Criar externalConnection</span><span class="sxs-lookup"><span data-stu-id="a6e81-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="a6e81-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="a6e81-111">externalConnection</span></span>                            | <span data-ttu-id="a6e81-112">Crie um novo externalConnection postando na coleção Connections.</span><span class="sxs-lookup"><span data-stu-id="a6e81-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="a6e81-113">Listar externalConnections</span><span class="sxs-lookup"><span data-stu-id="a6e81-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="a6e81-114">coleção externalConnection</span><span class="sxs-lookup"><span data-stu-id="a6e81-114">externalConnection collection</span></span>                 | <span data-ttu-id="a6e81-115">Obtenha uma coleção de objetos externalConnection.</span><span class="sxs-lookup"><span data-stu-id="a6e81-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="a6e81-116">Obter externalConnection</span><span class="sxs-lookup"><span data-stu-id="a6e81-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="a6e81-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="a6e81-117">externalConnection</span></span>                            | <span data-ttu-id="a6e81-118">Ler propriedades e relações de um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="a6e81-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="a6e81-119">Atualizar externalConnection</span><span class="sxs-lookup"><span data-stu-id="a6e81-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="a6e81-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="a6e81-120">externalConnection</span></span>                            | <span data-ttu-id="a6e81-121">Atualizar um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="a6e81-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="a6e81-122">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="a6e81-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="a6e81-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6e81-123">None</span></span>                                          | <span data-ttu-id="a6e81-124">Excluir um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="a6e81-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="a6e81-125">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="a6e81-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="a6e81-126">Nenhum *ou* [esquema](schema.md)</span><span class="sxs-lookup"><span data-stu-id="a6e81-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="a6e81-127">Registrar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="a6e81-127">Register connection schema.</span></span> |
| [<span data-ttu-id="a6e81-128">Operação get</span><span class="sxs-lookup"><span data-stu-id="a6e81-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="a6e81-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="a6e81-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="a6e81-130">Obter o status de uma solicitação assíncrona para criar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="a6e81-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="a6e81-131">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="a6e81-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="a6e81-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="a6e81-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="a6e81-133">Criar um novo externalItem postando na coleção Items.</span><span class="sxs-lookup"><span data-stu-id="a6e81-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="a6e81-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6e81-134">Properties</span></span>

| <span data-ttu-id="a6e81-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6e81-135">Property</span></span>      | <span data-ttu-id="a6e81-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6e81-136">Type</span></span>                              | <span data-ttu-id="a6e81-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6e81-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="a6e81-138">configuration</span><span class="sxs-lookup"><span data-stu-id="a6e81-138">configuration</span></span> | [<span data-ttu-id="a6e81-139">configuration</span><span class="sxs-lookup"><span data-stu-id="a6e81-139">configuration</span></span>](configuration.md) | <span data-ttu-id="a6e81-140">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar o conteúdo na conexão.</span><span class="sxs-lookup"><span data-stu-id="a6e81-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="a6e81-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a6e81-141">Optional.</span></span> |
| <span data-ttu-id="a6e81-142">description</span><span class="sxs-lookup"><span data-stu-id="a6e81-142">description</span></span>   | <span data-ttu-id="a6e81-143">String</span><span class="sxs-lookup"><span data-stu-id="a6e81-143">String</span></span>                            | <span data-ttu-id="a6e81-144">Descrição da conexão exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a6e81-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="a6e81-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a6e81-145">Optional.</span></span> |
| <span data-ttu-id="a6e81-146">id</span><span class="sxs-lookup"><span data-stu-id="a6e81-146">id</span></span>            | <span data-ttu-id="a6e81-147">String</span><span class="sxs-lookup"><span data-stu-id="a6e81-147">String</span></span>                            | <span data-ttu-id="a6e81-148">ID exclusiva fornecida pelo desenvolvedor da conexão dentro do locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a6e81-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="a6e81-149">Comprimento máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="a6e81-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="a6e81-150">Deve conter apenas caracteres alfanuméricos.</span><span class="sxs-lookup"><span data-stu-id="a6e81-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="a6e81-151">Não pode começar com `Microsoft` um dos seguintes valores:,, `None` `Directory` ,, `Exchange` `ExchangeArchive` `LinkedIn` , `Mailbox` , `MicrosoftSearch` , `OneDriveBusiness` ,,, `SharePoint` , `Teams` `Yammer` `Connectors` ,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="a6e81-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="a6e81-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6e81-152">Required.</span></span> |
| <span data-ttu-id="a6e81-153">nome</span><span class="sxs-lookup"><span data-stu-id="a6e81-153">name</span></span>          | <span data-ttu-id="a6e81-154">String</span><span class="sxs-lookup"><span data-stu-id="a6e81-154">String</span></span>                            | <span data-ttu-id="a6e81-155">O nome de exibição da conexão a ser exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a6e81-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="a6e81-156">Comprimento máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="a6e81-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="a6e81-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6e81-157">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a6e81-158">Relações</span><span class="sxs-lookup"><span data-stu-id="a6e81-158">Relationships</span></span>

| <span data-ttu-id="a6e81-159">Relação</span><span class="sxs-lookup"><span data-stu-id="a6e81-159">Relationship</span></span> | <span data-ttu-id="a6e81-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6e81-160">Type</span></span>                                                     | <span data-ttu-id="a6e81-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6e81-161">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="a6e81-162">items</span><span class="sxs-lookup"><span data-stu-id="a6e81-162">items</span></span>        | <span data-ttu-id="a6e81-163">coleção [externalItem](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="a6e81-163">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="a6e81-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="a6e81-p105">Read-only. Nullable.</span></span> |
| <span data-ttu-id="a6e81-166">operations</span><span class="sxs-lookup"><span data-stu-id="a6e81-166">operations</span></span>   | <span data-ttu-id="a6e81-167">coleção [connectionOperation](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="a6e81-167">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="a6e81-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6e81-168">Read-only.</span></span> <span data-ttu-id="a6e81-169">Anulável.</span><span class="sxs-lookup"><span data-stu-id="a6e81-169">Nullable.</span></span> |
| <span data-ttu-id="a6e81-170">esquemas</span><span class="sxs-lookup"><span data-stu-id="a6e81-170">schema</span></span>       | [<span data-ttu-id="a6e81-171">schema</span><span class="sxs-lookup"><span data-stu-id="a6e81-171">schema</span></span>](schema.md)                                      | <span data-ttu-id="a6e81-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="a6e81-p107">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6e81-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6e81-174">JSON representation</span></span>

<span data-ttu-id="a6e81-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6e81-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "configuration": {"@odata.type": "microsoft.graph.configuration"},
  "description": "String",
  "id": "String (identifier)",
  "name": "String"
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


