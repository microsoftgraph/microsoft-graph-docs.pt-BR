---
title: tipo de recurso externalConnection
description: Uma conexão com a Microsoft Search a partir de uma fonte externa.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4a77afc0aeef6c68d7bd58e554848068f25e1142
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866837"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="479d5-103">tipo de recurso externalConnection</span><span class="sxs-lookup"><span data-stu-id="479d5-103">externalConnection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="479d5-104">Uma conexão com a Microsoft Search a partir de uma fonte externa.</span><span class="sxs-lookup"><span data-stu-id="479d5-104">A connection to Microsoft Search from an external source.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="479d5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="479d5-105">Methods</span></span>

| <span data-ttu-id="479d5-106">Método</span><span class="sxs-lookup"><span data-stu-id="479d5-106">Method</span></span>                                                           | <span data-ttu-id="479d5-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="479d5-107">Return Type</span></span>                                   | <span data-ttu-id="479d5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="479d5-108">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="479d5-109">Criar externalConnection</span><span class="sxs-lookup"><span data-stu-id="479d5-109">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="479d5-110">externalConnection</span><span class="sxs-lookup"><span data-stu-id="479d5-110">externalConnection</span></span>                            | <span data-ttu-id="479d5-111">Crie um novo externalConnection postando na coleção Connections.</span><span class="sxs-lookup"><span data-stu-id="479d5-111">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="479d5-112">Listar externalConnections</span><span class="sxs-lookup"><span data-stu-id="479d5-112">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="479d5-113">coleção externalConnection</span><span class="sxs-lookup"><span data-stu-id="479d5-113">externalConnection collection</span></span>                 | <span data-ttu-id="479d5-114">Obtenha uma coleção de objetos externalConnection.</span><span class="sxs-lookup"><span data-stu-id="479d5-114">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="479d5-115">Obter externalConnection</span><span class="sxs-lookup"><span data-stu-id="479d5-115">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="479d5-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="479d5-116">externalConnection</span></span>                            | <span data-ttu-id="479d5-117">Ler propriedades e relações de um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="479d5-117">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="479d5-118">Atualizar externalConnection</span><span class="sxs-lookup"><span data-stu-id="479d5-118">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="479d5-119">externalConnection</span><span class="sxs-lookup"><span data-stu-id="479d5-119">externalConnection</span></span>                            | <span data-ttu-id="479d5-120">Atualizar um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="479d5-120">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="479d5-121">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="479d5-121">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="479d5-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="479d5-122">None</span></span>                                          | <span data-ttu-id="479d5-123">Excluir um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="479d5-123">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="479d5-124">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="479d5-124">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="479d5-125">Nenhum *ou* [esquema](schema.md)</span><span class="sxs-lookup"><span data-stu-id="479d5-125">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="479d5-126">Registrar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="479d5-126">Register connection schema.</span></span> |
| [<span data-ttu-id="479d5-127">Operação get</span><span class="sxs-lookup"><span data-stu-id="479d5-127">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="479d5-128">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="479d5-128">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="479d5-129">Obter o status de uma solicitação assíncrona para criar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="479d5-129">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="479d5-130">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="479d5-130">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="479d5-131">externalItem</span><span class="sxs-lookup"><span data-stu-id="479d5-131">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="479d5-132">Criar um novo externalItem postando na coleção Items.</span><span class="sxs-lookup"><span data-stu-id="479d5-132">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="479d5-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="479d5-133">Properties</span></span>

| <span data-ttu-id="479d5-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="479d5-134">Property</span></span>      | <span data-ttu-id="479d5-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="479d5-135">Type</span></span>                              | <span data-ttu-id="479d5-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="479d5-136">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="479d5-137">Configuration</span><span class="sxs-lookup"><span data-stu-id="479d5-137">configuration</span></span> | [<span data-ttu-id="479d5-138">configuration</span><span class="sxs-lookup"><span data-stu-id="479d5-138">configuration</span></span>](configuration.md) | <span data-ttu-id="479d5-139">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar o conteúdo na conexão.</span><span class="sxs-lookup"><span data-stu-id="479d5-139">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="479d5-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="479d5-140">Optional.</span></span> |
| <span data-ttu-id="479d5-141">descrição</span><span class="sxs-lookup"><span data-stu-id="479d5-141">description</span></span>   | <span data-ttu-id="479d5-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="479d5-142">String</span></span>                            | <span data-ttu-id="479d5-143">Descrição da conexão exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="479d5-143">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="479d5-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="479d5-144">Optional.</span></span> |
| <span data-ttu-id="479d5-145">id</span><span class="sxs-lookup"><span data-stu-id="479d5-145">id</span></span>            | <span data-ttu-id="479d5-146">String</span><span class="sxs-lookup"><span data-stu-id="479d5-146">String</span></span>                            | <span data-ttu-id="479d5-147">ID exclusiva fornecida pelo desenvolvedor da conexão dentro do locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="479d5-147">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="479d5-148">Comprimento máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="479d5-148">Maximum length of 32 characters.</span></span> <span data-ttu-id="479d5-149">Deve conter apenas caracteres alfanuméricos.</span><span class="sxs-lookup"><span data-stu-id="479d5-149">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="479d5-150">Não pode começar `Microsoft` com um dos seguintes valores: `None` `Directory`,, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`,,, `Yammer`, `Connectors`,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="479d5-150">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="479d5-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="479d5-151">Required.</span></span> |
| <span data-ttu-id="479d5-152">nome</span><span class="sxs-lookup"><span data-stu-id="479d5-152">name</span></span>          | <span data-ttu-id="479d5-153">String</span><span class="sxs-lookup"><span data-stu-id="479d5-153">String</span></span>                            | <span data-ttu-id="479d5-154">O nome de exibição da conexão a ser exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="479d5-154">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="479d5-155">Comprimento máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="479d5-155">Maximum length of 128 characters.</span></span> <span data-ttu-id="479d5-156">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="479d5-156">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="479d5-157">Relações</span><span class="sxs-lookup"><span data-stu-id="479d5-157">Relationships</span></span>

| <span data-ttu-id="479d5-158">Relação</span><span class="sxs-lookup"><span data-stu-id="479d5-158">Relationship</span></span> | <span data-ttu-id="479d5-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="479d5-159">Type</span></span>                                                     | <span data-ttu-id="479d5-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="479d5-160">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="479d5-161">items</span><span class="sxs-lookup"><span data-stu-id="479d5-161">items</span></span>        | <span data-ttu-id="479d5-162">coleção [externalItem](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="479d5-162">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="479d5-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="479d5-p105">Read-only. Nullable.</span></span> |
| <span data-ttu-id="479d5-165">operations</span><span class="sxs-lookup"><span data-stu-id="479d5-165">operations</span></span>   | <span data-ttu-id="479d5-166">coleção [connectionOperation](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="479d5-166">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="479d5-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="479d5-167">Read-only.</span></span> <span data-ttu-id="479d5-168">Anulável.</span><span class="sxs-lookup"><span data-stu-id="479d5-168">Nullable.</span></span> |
| <span data-ttu-id="479d5-169">esquemas</span><span class="sxs-lookup"><span data-stu-id="479d5-169">schema</span></span>       | [<span data-ttu-id="479d5-170">schema</span><span class="sxs-lookup"><span data-stu-id="479d5-170">schema</span></span>](schema.md)                                      | <span data-ttu-id="479d5-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="479d5-p107">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="479d5-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="479d5-173">JSON representation</span></span>

<span data-ttu-id="479d5-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="479d5-174">The following is a JSON representation of the resource.</span></span>

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
