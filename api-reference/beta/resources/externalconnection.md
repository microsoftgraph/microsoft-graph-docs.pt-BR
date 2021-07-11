---
title: Tipo de recurso externalConnection
description: Uma conexão é um contêiner lógico para seu conteúdo externo no Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4b0c0a56fc415c4f2f75ec4972909e31fc9bea14
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366566"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="06984-103">Tipo de recurso externalConnection</span><span class="sxs-lookup"><span data-stu-id="06984-103">externalConnection resource type</span></span>

<span data-ttu-id="06984-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06984-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06984-105">Um contêiner lógico para adicionar conteúdo de uma fonte externa à Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="06984-105">A logical container to add content from an external source into Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="06984-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="06984-106">Methods</span></span>

| <span data-ttu-id="06984-107">Método</span><span class="sxs-lookup"><span data-stu-id="06984-107">Method</span></span>                                                           | <span data-ttu-id="06984-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="06984-108">Return Type</span></span>                                   | <span data-ttu-id="06984-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="06984-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="06984-110">Criar externalConnection</span><span class="sxs-lookup"><span data-stu-id="06984-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="06984-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="06984-111">externalConnection</span></span>                            | <span data-ttu-id="06984-112">Crie um novo externalConnection postando na coleção connections.</span><span class="sxs-lookup"><span data-stu-id="06984-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="06984-113">Listar externalConnections</span><span class="sxs-lookup"><span data-stu-id="06984-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="06984-114">Coleção externalConnection</span><span class="sxs-lookup"><span data-stu-id="06984-114">externalConnection collection</span></span>                 | <span data-ttu-id="06984-115">Obter uma coleção de objetos externalConnection.</span><span class="sxs-lookup"><span data-stu-id="06984-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="06984-116">Obter externalConnection</span><span class="sxs-lookup"><span data-stu-id="06984-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="06984-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="06984-117">externalConnection</span></span>                            | <span data-ttu-id="06984-118">Ler propriedades e relações de um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="06984-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="06984-119">Atualizar externalConnection</span><span class="sxs-lookup"><span data-stu-id="06984-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="06984-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="06984-120">externalConnection</span></span>                            | <span data-ttu-id="06984-121">Atualize um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="06984-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="06984-122">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="06984-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="06984-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06984-123">None</span></span>                                          | <span data-ttu-id="06984-124">Exclua um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="06984-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="06984-125">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="06984-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="06984-126">Nenhum *ou* [esquema](schema.md)</span><span class="sxs-lookup"><span data-stu-id="06984-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="06984-127">Registrar esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="06984-127">Register connection schema.</span></span> |
| [<span data-ttu-id="06984-128">Obter operação</span><span class="sxs-lookup"><span data-stu-id="06984-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="06984-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="06984-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="06984-130">Obter o status de uma solicitação assíncrona para criar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="06984-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="06984-131">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="06984-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="06984-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="06984-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="06984-133">Crie um novo externalItem postando na coleção items.</span><span class="sxs-lookup"><span data-stu-id="06984-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="06984-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06984-134">Properties</span></span>

| <span data-ttu-id="06984-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06984-135">Property</span></span>      | <span data-ttu-id="06984-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="06984-136">Type</span></span>                              | <span data-ttu-id="06984-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="06984-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="06984-138">configuração</span><span class="sxs-lookup"><span data-stu-id="06984-138">configuration</span></span> | [<span data-ttu-id="06984-139">configuration</span><span class="sxs-lookup"><span data-stu-id="06984-139">configuration</span></span>](configuration.md) | <span data-ttu-id="06984-140">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar conteúdo na conexão.</span><span class="sxs-lookup"><span data-stu-id="06984-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="06984-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="06984-141">Optional.</span></span> |
| <span data-ttu-id="06984-142">descrição</span><span class="sxs-lookup"><span data-stu-id="06984-142">description</span></span>   | <span data-ttu-id="06984-143">String</span><span class="sxs-lookup"><span data-stu-id="06984-143">String</span></span>                            | <span data-ttu-id="06984-144">Descrição da conexão exibida no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="06984-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="06984-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="06984-145">Optional.</span></span> |
| <span data-ttu-id="06984-146">id</span><span class="sxs-lookup"><span data-stu-id="06984-146">id</span></span>            | <span data-ttu-id="06984-147">String</span><span class="sxs-lookup"><span data-stu-id="06984-147">String</span></span>                            | <span data-ttu-id="06984-148">ID exclusiva fornecida pelo desenvolvedor da conexão no Azure Active Directory locatário.</span><span class="sxs-lookup"><span data-stu-id="06984-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="06984-149">Comprimento máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="06984-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="06984-150">Deve conter somente caracteres alfanuméricos.</span><span class="sxs-lookup"><span data-stu-id="06984-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="06984-151">Não é possível `Microsoft` começar ou ser um dos seguintes valores: , , , `None` , , , , , , , , `Directory` , , `Exchange` , `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` .</span><span class="sxs-lookup"><span data-stu-id="06984-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="06984-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06984-152">Required.</span></span> |
| <span data-ttu-id="06984-153">nome</span><span class="sxs-lookup"><span data-stu-id="06984-153">name</span></span>          | <span data-ttu-id="06984-154">String</span><span class="sxs-lookup"><span data-stu-id="06984-154">String</span></span>                            | <span data-ttu-id="06984-155">O nome de exibição da conexão a ser exibida no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="06984-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="06984-156">Comprimento máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="06984-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="06984-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06984-157">Required.</span></span> |
| <span data-ttu-id="06984-158">state</span><span class="sxs-lookup"><span data-stu-id="06984-158">state</span></span>         | <span data-ttu-id="06984-159">connectionState</span><span class="sxs-lookup"><span data-stu-id="06984-159">connectionState</span></span>                   | <span data-ttu-id="06984-160">Indica o estado atual da conexão.</span><span class="sxs-lookup"><span data-stu-id="06984-160">Indicates the current state of the connection.</span></span> <span data-ttu-id="06984-161">Os valores possíveis `draft` `ready` são , e `obsolete` `limitExceeded` .</span><span class="sxs-lookup"><span data-stu-id="06984-161">Possible values are `draft`, `ready`, `obsolete`, and `limitExceeded`.</span></span> <span data-ttu-id="06984-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06984-162">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="06984-163">Relações</span><span class="sxs-lookup"><span data-stu-id="06984-163">Relationships</span></span>

| <span data-ttu-id="06984-164">Relação</span><span class="sxs-lookup"><span data-stu-id="06984-164">Relationship</span></span> | <span data-ttu-id="06984-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="06984-165">Type</span></span>                                                     | <span data-ttu-id="06984-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="06984-166">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="06984-167">items</span><span class="sxs-lookup"><span data-stu-id="06984-167">items</span></span>        | <span data-ttu-id="06984-168">[Coleção externalItem](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="06984-168">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="06984-p106">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="06984-p106">Read-only. Nullable.</span></span> |
| <span data-ttu-id="06984-171">operations</span><span class="sxs-lookup"><span data-stu-id="06984-171">operations</span></span>   | <span data-ttu-id="06984-172">[Coleção connectionOperation](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="06984-172">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="06984-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="06984-p107">Read-only. Nullable.</span></span> |
| <span data-ttu-id="06984-175">esquema</span><span class="sxs-lookup"><span data-stu-id="06984-175">schema</span></span>       | [<span data-ttu-id="06984-176">schema</span><span class="sxs-lookup"><span data-stu-id="06984-176">schema</span></span>](schema.md)                                      | <span data-ttu-id="06984-p108">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="06984-p108">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="06984-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06984-179">JSON representation</span></span>

<span data-ttu-id="06984-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06984-180">The following is a JSON representation of the resource.</span></span>

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
