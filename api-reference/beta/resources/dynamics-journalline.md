---
title: tipo de recurso journalLines
description: Uma linha de diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 99d06b5a49bd2881ea6f329e8b0d3692a25444b4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013794"
---
# <a name="journallines-resource-type"></a><span data-ttu-id="ba93e-103">tipo de recurso journalLines</span><span class="sxs-lookup"><span data-stu-id="ba93e-103">journalLines resource type</span></span>

<span data-ttu-id="ba93e-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ba93e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba93e-105">Representa uma linha em um diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="ba93e-105">Represents a line in a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="ba93e-106">Methods</span><span class="sxs-lookup"><span data-stu-id="ba93e-106">Methods</span></span>

| <span data-ttu-id="ba93e-107">Método</span><span class="sxs-lookup"><span data-stu-id="ba93e-107">Method</span></span>                                                    | <span data-ttu-id="ba93e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ba93e-108">Return Type</span></span>|<span data-ttu-id="ba93e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba93e-109">Description</span></span>         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[<span data-ttu-id="ba93e-110">Obter journalLines</span><span class="sxs-lookup"><span data-stu-id="ba93e-110">Get journalLines</span></span>](../api/dynamics-journalline-get.md)      |<span data-ttu-id="ba93e-111">journalLines</span><span class="sxs-lookup"><span data-stu-id="ba93e-111">journalLines</span></span>|<span data-ttu-id="ba93e-112">Obtém uma linha do diário.</span><span class="sxs-lookup"><span data-stu-id="ba93e-112">Gets a journal line.</span></span>   |
|[<span data-ttu-id="ba93e-113">Postar journalLines</span><span class="sxs-lookup"><span data-stu-id="ba93e-113">Post journalLines</span></span>](../api/dynamics-create-journalline.md)  |<span data-ttu-id="ba93e-114">journalLines</span><span class="sxs-lookup"><span data-stu-id="ba93e-114">journalLines</span></span>|<span data-ttu-id="ba93e-115">Cria uma linha de diário.</span><span class="sxs-lookup"><span data-stu-id="ba93e-115">Creates a journal line.</span></span>|
|[<span data-ttu-id="ba93e-116">Patch journalLines</span><span class="sxs-lookup"><span data-stu-id="ba93e-116">Patch journalLines</span></span>](../api/dynamics-journalline-update.md) |<span data-ttu-id="ba93e-117">journalLines</span><span class="sxs-lookup"><span data-stu-id="ba93e-117">journalLines</span></span>|<span data-ttu-id="ba93e-118">Atualiza uma linha do diário.</span><span class="sxs-lookup"><span data-stu-id="ba93e-118">Updates a journal line.</span></span>|
|[<span data-ttu-id="ba93e-119">Excluir journalLines</span><span class="sxs-lookup"><span data-stu-id="ba93e-119">Delete journalLines</span></span>](../api/dynamics-journalline-delete.md)|<span data-ttu-id="ba93e-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ba93e-120">none</span></span>        |<span data-ttu-id="ba93e-121">Exclui uma linha do diário.</span><span class="sxs-lookup"><span data-stu-id="ba93e-121">Deletes a journal line.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba93e-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba93e-122">Properties</span></span>
| <span data-ttu-id="ba93e-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba93e-123">Property</span></span>             | <span data-ttu-id="ba93e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba93e-124">Type</span></span>                   |<span data-ttu-id="ba93e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba93e-125">Description</span></span>                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|<span data-ttu-id="ba93e-126">id</span><span class="sxs-lookup"><span data-stu-id="ba93e-126">id</span></span>                    |<span data-ttu-id="ba93e-127">GUID</span><span class="sxs-lookup"><span data-stu-id="ba93e-127">GUID</span></span>                    |<span data-ttu-id="ba93e-128">A identificação exclusiva da linha do diário.</span><span class="sxs-lookup"><span data-stu-id="ba93e-128">The unique ID of the journal line.</span></span> <span data-ttu-id="ba93e-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="ba93e-129">Non-editable.</span></span>                   |
|<span data-ttu-id="ba93e-130">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="ba93e-130">journalDisplayName</span></span>    |<span data-ttu-id="ba93e-131">Cadeia de caracteres, tamanho máximo 10</span><span class="sxs-lookup"><span data-stu-id="ba93e-131">string, maximum size 10</span></span> |<span data-ttu-id="ba93e-132">O nome de exibição do diário ao qual esta linha pertence.</span><span class="sxs-lookup"><span data-stu-id="ba93e-132">The display name of the journal that this line belongs to.</span></span> <span data-ttu-id="ba93e-133">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="ba93e-133">Read-Only.</span></span>|
|<span data-ttu-id="ba93e-134">lineNumber</span><span class="sxs-lookup"><span data-stu-id="ba93e-134">lineNumber</span></span>            |<span data-ttu-id="ba93e-135">inteiro</span><span class="sxs-lookup"><span data-stu-id="ba93e-135">integer</span></span>                 |<span data-ttu-id="ba93e-136">O número da linha do diário.</span><span class="sxs-lookup"><span data-stu-id="ba93e-136">The number of the journal line.</span></span>                                    |
|<span data-ttu-id="ba93e-137">accountId</span><span class="sxs-lookup"><span data-stu-id="ba93e-137">accountId</span></span>             |<span data-ttu-id="ba93e-138">GUID</span><span class="sxs-lookup"><span data-stu-id="ba93e-138">GUID</span></span>                    |<span data-ttu-id="ba93e-139">A identificação exclusiva da conta à qual a linha do diário está relacionada.</span><span class="sxs-lookup"><span data-stu-id="ba93e-139">The unique ID of the account that the journal line is related to.</span></span>  |
|<span data-ttu-id="ba93e-140">accountNumber</span><span class="sxs-lookup"><span data-stu-id="ba93e-140">accountNumber</span></span>         |<span data-ttu-id="ba93e-141">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="ba93e-141">string, maximum size 20</span></span> |<span data-ttu-id="ba93e-142">O número da conta à qual a linha do diário está relacionada.</span><span class="sxs-lookup"><span data-stu-id="ba93e-142">The number of the account that the journal line is related to.</span></span>     |
|<span data-ttu-id="ba93e-143">postingDate</span><span class="sxs-lookup"><span data-stu-id="ba93e-143">postingDate</span></span>           |<span data-ttu-id="ba93e-144">data</span><span class="sxs-lookup"><span data-stu-id="ba93e-144">date</span></span>                    |<span data-ttu-id="ba93e-145">A data em que a linha do diário é lançada.</span><span class="sxs-lookup"><span data-stu-id="ba93e-145">The date that the journal line is posted.</span></span>                          |
|<span data-ttu-id="ba93e-146">documentNumber</span><span class="sxs-lookup"><span data-stu-id="ba93e-146">documentNumber</span></span>        |<span data-ttu-id="ba93e-147">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="ba93e-147">string, maximum size 20</span></span> |<span data-ttu-id="ba93e-148">Especifica um número de documento para a linha do diário.</span><span class="sxs-lookup"><span data-stu-id="ba93e-148">Specifies a document number for the journal line.</span></span>                  |
|<span data-ttu-id="ba93e-149">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="ba93e-149">externalDocumentNumber</span></span>|<span data-ttu-id="ba93e-150">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="ba93e-150">string, maximum size 20</span></span> |<span data-ttu-id="ba93e-151">Especifica um número de documento externo para a linha do diário.</span><span class="sxs-lookup"><span data-stu-id="ba93e-151">Specifies an external document number for the journal line.</span></span>        |
|<span data-ttu-id="ba93e-152">quantia</span><span class="sxs-lookup"><span data-stu-id="ba93e-152">amount</span></span>                |<span data-ttu-id="ba93e-153">dígitos</span><span class="sxs-lookup"><span data-stu-id="ba93e-153">decimal</span></span>                 |<span data-ttu-id="ba93e-154">Especifica o valor total (incluindo o IVA) que a linha do diário consiste.</span><span class="sxs-lookup"><span data-stu-id="ba93e-154">Specifies the total amount (including VAT) that the journal line consists of.</span></span>|
|<span data-ttu-id="ba93e-155">description</span><span class="sxs-lookup"><span data-stu-id="ba93e-155">description</span></span>           |<span data-ttu-id="ba93e-156">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="ba93e-156">string, maximum size 50</span></span> |<span data-ttu-id="ba93e-157">A descrição da linha do diário, fornecida pelo usuário ou autocriada.</span><span class="sxs-lookup"><span data-stu-id="ba93e-157">The description of the journal line, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="ba93e-158">comment</span><span class="sxs-lookup"><span data-stu-id="ba93e-158">comment</span></span>               |<span data-ttu-id="ba93e-159">Cadeia de caracteres, tamanho máximo 250</span><span class="sxs-lookup"><span data-stu-id="ba93e-159">string, maximum size 250</span></span>|<span data-ttu-id="ba93e-160">Um comentário especificado pelo usuário na linha do diário.</span><span class="sxs-lookup"><span data-stu-id="ba93e-160">A user specified comment on the journal line.</span></span>                      |
|<span data-ttu-id="ba93e-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba93e-161">lastModifiedDateTime</span></span>  |<span data-ttu-id="ba93e-162">datetime</span><span class="sxs-lookup"><span data-stu-id="ba93e-162">datetime</span></span>                |<span data-ttu-id="ba93e-163">O último DateTime em que a linha do diário foi modificada.</span><span class="sxs-lookup"><span data-stu-id="ba93e-163">The last datetime the journal line was modified.</span></span> <span data-ttu-id="ba93e-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ba93e-164">Read-Only.</span></span>        |

## <a name="relationships"></a><span data-ttu-id="ba93e-165">Relações</span><span class="sxs-lookup"><span data-stu-id="ba93e-165">Relationships</span></span>
<span data-ttu-id="ba93e-166">Uma linha de diário é uma subpágina de um diário.</span><span class="sxs-lookup"><span data-stu-id="ba93e-166">A journal line is a subpage of a journal.</span></span> <span data-ttu-id="ba93e-167">Ele não pode ser acessado diretamente.</span><span class="sxs-lookup"><span data-stu-id="ba93e-167">It cannot be accessed directly.</span></span>

<span data-ttu-id="ba93e-168">Uma linha de diário pode ser uma "entidade pai" das linhas de dimensão.</span><span class="sxs-lookup"><span data-stu-id="ba93e-168">A journal line can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="ba93e-169">Uma conta (AccountId) deve existir na tabela accounts.</span><span class="sxs-lookup"><span data-stu-id="ba93e-169">An Account (accountId) must exist in the Accounts table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ba93e-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba93e-170">JSON representation</span></span>

<span data-ttu-id="ba93e-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba93e-171">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "accountId": "GUID",
    "accountNumber": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```


