---
title: tipo de recurso externalConnection
description: Uma conexão com a Microsoft Search a partir de uma fonte externa.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 49e268f894b6733eb3f44d36fa34bc7c80df0ded
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498914"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="25656-103">tipo de recurso externalConnection</span><span class="sxs-lookup"><span data-stu-id="25656-103">externalConnection resource type</span></span>

<span data-ttu-id="25656-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="25656-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25656-105">Uma conexão com a Microsoft Search a partir de uma fonte externa.</span><span class="sxs-lookup"><span data-stu-id="25656-105">A connection to Microsoft Search from an external source.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="25656-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="25656-106">Methods</span></span>

| <span data-ttu-id="25656-107">Método</span><span class="sxs-lookup"><span data-stu-id="25656-107">Method</span></span>                                                           | <span data-ttu-id="25656-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="25656-108">Return Type</span></span>                                   | <span data-ttu-id="25656-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="25656-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="25656-110">Criar externalConnection</span><span class="sxs-lookup"><span data-stu-id="25656-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="25656-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="25656-111">externalConnection</span></span>                            | <span data-ttu-id="25656-112">Crie um novo externalConnection postando na coleção Connections.</span><span class="sxs-lookup"><span data-stu-id="25656-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="25656-113">Listar externalConnections</span><span class="sxs-lookup"><span data-stu-id="25656-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="25656-114">coleção externalConnection</span><span class="sxs-lookup"><span data-stu-id="25656-114">externalConnection collection</span></span>                 | <span data-ttu-id="25656-115">Obtenha uma coleção de objetos externalConnection.</span><span class="sxs-lookup"><span data-stu-id="25656-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="25656-116">Obter externalConnection</span><span class="sxs-lookup"><span data-stu-id="25656-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="25656-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="25656-117">externalConnection</span></span>                            | <span data-ttu-id="25656-118">Ler propriedades e relações de um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="25656-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="25656-119">Atualizar externalConnection</span><span class="sxs-lookup"><span data-stu-id="25656-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="25656-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="25656-120">externalConnection</span></span>                            | <span data-ttu-id="25656-121">Atualizar um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="25656-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="25656-122">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="25656-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="25656-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25656-123">None</span></span>                                          | <span data-ttu-id="25656-124">Excluir um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="25656-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="25656-125">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="25656-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="25656-126">Nenhum *ou* [esquema](schema.md)</span><span class="sxs-lookup"><span data-stu-id="25656-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="25656-127">Registrar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="25656-127">Register connection schema.</span></span> |
| [<span data-ttu-id="25656-128">Operação get</span><span class="sxs-lookup"><span data-stu-id="25656-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="25656-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="25656-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="25656-130">Obter o status de uma solicitação assíncrona para criar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="25656-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="25656-131">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="25656-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="25656-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="25656-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="25656-133">Criar um novo externalItem postando na coleção Items.</span><span class="sxs-lookup"><span data-stu-id="25656-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="25656-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25656-134">Properties</span></span>

| <span data-ttu-id="25656-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25656-135">Property</span></span>      | <span data-ttu-id="25656-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="25656-136">Type</span></span>                              | <span data-ttu-id="25656-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="25656-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="25656-138">Configuration</span><span class="sxs-lookup"><span data-stu-id="25656-138">configuration</span></span> | [<span data-ttu-id="25656-139">configuration</span><span class="sxs-lookup"><span data-stu-id="25656-139">configuration</span></span>](configuration.md) | <span data-ttu-id="25656-140">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar o conteúdo na conexão.</span><span class="sxs-lookup"><span data-stu-id="25656-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="25656-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="25656-141">Optional.</span></span> |
| <span data-ttu-id="25656-142">description</span><span class="sxs-lookup"><span data-stu-id="25656-142">description</span></span>   | <span data-ttu-id="25656-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25656-143">String</span></span>                            | <span data-ttu-id="25656-144">Descrição da conexão exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="25656-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="25656-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="25656-145">Optional.</span></span> |
| <span data-ttu-id="25656-146">id</span><span class="sxs-lookup"><span data-stu-id="25656-146">id</span></span>            | <span data-ttu-id="25656-147">String</span><span class="sxs-lookup"><span data-stu-id="25656-147">String</span></span>                            | <span data-ttu-id="25656-148">ID exclusiva fornecida pelo desenvolvedor da conexão dentro do locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="25656-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="25656-149">Comprimento máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="25656-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="25656-150">Deve conter apenas caracteres alfanuméricos.</span><span class="sxs-lookup"><span data-stu-id="25656-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="25656-151">Não pode começar `Microsoft` com um dos seguintes valores: `None` `Directory`,, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`,,, `Yammer`, `Connectors`,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="25656-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="25656-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25656-152">Required.</span></span> |
| <span data-ttu-id="25656-153">nome</span><span class="sxs-lookup"><span data-stu-id="25656-153">name</span></span>          | <span data-ttu-id="25656-154">String</span><span class="sxs-lookup"><span data-stu-id="25656-154">String</span></span>                            | <span data-ttu-id="25656-155">O nome de exibição da conexão a ser exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="25656-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="25656-156">Comprimento máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="25656-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="25656-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25656-157">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="25656-158">Relações</span><span class="sxs-lookup"><span data-stu-id="25656-158">Relationships</span></span>

| <span data-ttu-id="25656-159">Relação</span><span class="sxs-lookup"><span data-stu-id="25656-159">Relationship</span></span> | <span data-ttu-id="25656-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="25656-160">Type</span></span>                                                     | <span data-ttu-id="25656-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="25656-161">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="25656-162">items</span><span class="sxs-lookup"><span data-stu-id="25656-162">items</span></span>        | <span data-ttu-id="25656-163">coleção [externalItem](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="25656-163">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="25656-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="25656-p105">Read-only. Nullable.</span></span> |
| <span data-ttu-id="25656-166">operations</span><span class="sxs-lookup"><span data-stu-id="25656-166">operations</span></span>   | <span data-ttu-id="25656-167">coleção [connectionOperation](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="25656-167">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="25656-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25656-168">Read-only.</span></span> <span data-ttu-id="25656-169">Anulável.</span><span class="sxs-lookup"><span data-stu-id="25656-169">Nullable.</span></span> |
| <span data-ttu-id="25656-170">esquemas</span><span class="sxs-lookup"><span data-stu-id="25656-170">schema</span></span>       | [<span data-ttu-id="25656-171">schema</span><span class="sxs-lookup"><span data-stu-id="25656-171">schema</span></span>](schema.md)                                      | <span data-ttu-id="25656-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="25656-p107">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="25656-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25656-174">JSON representation</span></span>

<span data-ttu-id="25656-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25656-175">The following is a JSON representation of the resource.</span></span>

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
