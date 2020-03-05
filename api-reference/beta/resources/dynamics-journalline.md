---
title: tipo de recurso journalLines
description: Uma linha de diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 8285a64b931ab18dac51cc20224877bbac74be90
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503653"
---
# <a name="journallines-resource-type"></a><span data-ttu-id="0223d-103">tipo de recurso journalLines</span><span class="sxs-lookup"><span data-stu-id="0223d-103">journalLines resource type</span></span>

<span data-ttu-id="0223d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0223d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0223d-105">Representa uma linha em um diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="0223d-105">Represents a line in a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="0223d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0223d-106">Methods</span></span>

| <span data-ttu-id="0223d-107">Método</span><span class="sxs-lookup"><span data-stu-id="0223d-107">Method</span></span>                                                    | <span data-ttu-id="0223d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0223d-108">Return Type</span></span>|<span data-ttu-id="0223d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0223d-109">Description</span></span>         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[<span data-ttu-id="0223d-110">Obter journalLines</span><span class="sxs-lookup"><span data-stu-id="0223d-110">Get journalLines</span></span>](../api/dynamics-journalline-get.md)      |<span data-ttu-id="0223d-111">journalLines</span><span class="sxs-lookup"><span data-stu-id="0223d-111">journalLines</span></span>|<span data-ttu-id="0223d-112">Obtém uma linha do diário.</span><span class="sxs-lookup"><span data-stu-id="0223d-112">Gets a journal line.</span></span>   |
|[<span data-ttu-id="0223d-113">Postar journalLines</span><span class="sxs-lookup"><span data-stu-id="0223d-113">Post journalLines</span></span>](../api/dynamics-create-journalline.md)  |<span data-ttu-id="0223d-114">journalLines</span><span class="sxs-lookup"><span data-stu-id="0223d-114">journalLines</span></span>|<span data-ttu-id="0223d-115">Cria uma linha de diário.</span><span class="sxs-lookup"><span data-stu-id="0223d-115">Creates a journal line.</span></span>|
|[<span data-ttu-id="0223d-116">Patch journalLines</span><span class="sxs-lookup"><span data-stu-id="0223d-116">Patch journalLines</span></span>](../api/dynamics-journalline-update.md) |<span data-ttu-id="0223d-117">journalLines</span><span class="sxs-lookup"><span data-stu-id="0223d-117">journalLines</span></span>|<span data-ttu-id="0223d-118">Atualiza uma linha do diário.</span><span class="sxs-lookup"><span data-stu-id="0223d-118">Updates a journal line.</span></span>|
|[<span data-ttu-id="0223d-119">Excluir journalLines</span><span class="sxs-lookup"><span data-stu-id="0223d-119">Delete journalLines</span></span>](../api/dynamics-journalline-delete.md)|<span data-ttu-id="0223d-120">nenhuma</span><span class="sxs-lookup"><span data-stu-id="0223d-120">none</span></span>        |<span data-ttu-id="0223d-121">Exclui uma linha do diário.</span><span class="sxs-lookup"><span data-stu-id="0223d-121">Deletes a journal line.</span></span>|

## <a name="properties"></a><span data-ttu-id="0223d-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0223d-122">Properties</span></span>
| <span data-ttu-id="0223d-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0223d-123">Property</span></span>             | <span data-ttu-id="0223d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0223d-124">Type</span></span>                   |<span data-ttu-id="0223d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0223d-125">Description</span></span>                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|<span data-ttu-id="0223d-126">id</span><span class="sxs-lookup"><span data-stu-id="0223d-126">id</span></span>                    |<span data-ttu-id="0223d-127">GUID</span><span class="sxs-lookup"><span data-stu-id="0223d-127">GUID</span></span>                    |<span data-ttu-id="0223d-128">A identificação exclusiva da linha do diário.</span><span class="sxs-lookup"><span data-stu-id="0223d-128">The unique ID of the journal line.</span></span> <span data-ttu-id="0223d-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="0223d-129">Non-editable.</span></span>                   |
|<span data-ttu-id="0223d-130">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="0223d-130">journalDisplayName</span></span>    |<span data-ttu-id="0223d-131">Cadeia de caracteres, tamanho máximo 10</span><span class="sxs-lookup"><span data-stu-id="0223d-131">string, maximum size 10</span></span> |<span data-ttu-id="0223d-132">O nome de exibição do diário ao qual esta linha pertence.</span><span class="sxs-lookup"><span data-stu-id="0223d-132">The display name of the journal that this line belongs to.</span></span> <span data-ttu-id="0223d-133">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="0223d-133">Read-Only.</span></span>|
|<span data-ttu-id="0223d-134">lineNumber</span><span class="sxs-lookup"><span data-stu-id="0223d-134">lineNumber</span></span>            |<span data-ttu-id="0223d-135">inteiro</span><span class="sxs-lookup"><span data-stu-id="0223d-135">integer</span></span>                 |<span data-ttu-id="0223d-136">O número da linha do diário.</span><span class="sxs-lookup"><span data-stu-id="0223d-136">The number of the journal line.</span></span>                                    |
|<span data-ttu-id="0223d-137">accountId</span><span class="sxs-lookup"><span data-stu-id="0223d-137">accountId</span></span>             |<span data-ttu-id="0223d-138">GUID</span><span class="sxs-lookup"><span data-stu-id="0223d-138">GUID</span></span>                    |<span data-ttu-id="0223d-139">A identificação exclusiva da conta à qual a linha do diário está relacionada.</span><span class="sxs-lookup"><span data-stu-id="0223d-139">The unique ID of the account that the journal line is related to.</span></span>  |
|<span data-ttu-id="0223d-140">accountNumber</span><span class="sxs-lookup"><span data-stu-id="0223d-140">accountNumber</span></span>         |<span data-ttu-id="0223d-141">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="0223d-141">string, maximum size 20</span></span> |<span data-ttu-id="0223d-142">O número da conta à qual a linha do diário está relacionada.</span><span class="sxs-lookup"><span data-stu-id="0223d-142">The number of the account that the journal line is related to.</span></span>     |
|<span data-ttu-id="0223d-143">postingDate</span><span class="sxs-lookup"><span data-stu-id="0223d-143">postingDate</span></span>           |<span data-ttu-id="0223d-144">data</span><span class="sxs-lookup"><span data-stu-id="0223d-144">date</span></span>                    |<span data-ttu-id="0223d-145">A data em que a linha do diário é lançada.</span><span class="sxs-lookup"><span data-stu-id="0223d-145">The date that the journal line is posted.</span></span>                          |
|<span data-ttu-id="0223d-146">documentNumber</span><span class="sxs-lookup"><span data-stu-id="0223d-146">documentNumber</span></span>        |<span data-ttu-id="0223d-147">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="0223d-147">string, maximum size 20</span></span> |<span data-ttu-id="0223d-148">Especifica um número de documento para a linha do diário.</span><span class="sxs-lookup"><span data-stu-id="0223d-148">Specifies a document number for the journal line.</span></span>                  |
|<span data-ttu-id="0223d-149">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="0223d-149">externalDocumentNumber</span></span>|<span data-ttu-id="0223d-150">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="0223d-150">string, maximum size 20</span></span> |<span data-ttu-id="0223d-151">Especifica um número de documento externo para a linha do diário.</span><span class="sxs-lookup"><span data-stu-id="0223d-151">Specifies an external document number for the journal line.</span></span>        |
|<span data-ttu-id="0223d-152">quantia</span><span class="sxs-lookup"><span data-stu-id="0223d-152">amount</span></span>                |<span data-ttu-id="0223d-153">dígitos</span><span class="sxs-lookup"><span data-stu-id="0223d-153">decimal</span></span>                 |<span data-ttu-id="0223d-154">Especifica o valor total (incluindo o IVA) que a linha do diário consiste.</span><span class="sxs-lookup"><span data-stu-id="0223d-154">Specifies the total amount (including VAT) that the journal line consists of.</span></span>|
|<span data-ttu-id="0223d-155">description</span><span class="sxs-lookup"><span data-stu-id="0223d-155">description</span></span>           |<span data-ttu-id="0223d-156">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="0223d-156">string, maximum size 50</span></span> |<span data-ttu-id="0223d-157">A descrição da linha do diário, fornecida pelo usuário ou autocriada.</span><span class="sxs-lookup"><span data-stu-id="0223d-157">The description of the journal line, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="0223d-158">comment</span><span class="sxs-lookup"><span data-stu-id="0223d-158">comment</span></span>               |<span data-ttu-id="0223d-159">Cadeia de caracteres, tamanho máximo 250</span><span class="sxs-lookup"><span data-stu-id="0223d-159">string, maximum size 250</span></span>|<span data-ttu-id="0223d-160">Um comentário especificado pelo usuário na linha do diário.</span><span class="sxs-lookup"><span data-stu-id="0223d-160">A user specified comment on the journal line.</span></span>                      |
|<span data-ttu-id="0223d-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0223d-161">lastModifiedDateTime</span></span>  |<span data-ttu-id="0223d-162">datetime</span><span class="sxs-lookup"><span data-stu-id="0223d-162">datetime</span></span>                |<span data-ttu-id="0223d-163">O último DateTime em que a linha do diário foi modificada.</span><span class="sxs-lookup"><span data-stu-id="0223d-163">The last datetime the journal line was modified.</span></span> <span data-ttu-id="0223d-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0223d-164">Read-Only.</span></span>        |

## <a name="relationships"></a><span data-ttu-id="0223d-165">Relações</span><span class="sxs-lookup"><span data-stu-id="0223d-165">Relationships</span></span>
<span data-ttu-id="0223d-166">Uma linha de diário é uma subpágina de um diário.</span><span class="sxs-lookup"><span data-stu-id="0223d-166">A journal line is a subpage of a journal.</span></span> <span data-ttu-id="0223d-167">Ele não pode ser acessado diretamente.</span><span class="sxs-lookup"><span data-stu-id="0223d-167">It cannot be accessed directly.</span></span>

<span data-ttu-id="0223d-168">Uma linha de diário pode ser uma "entidade pai" das linhas de dimensão.</span><span class="sxs-lookup"><span data-stu-id="0223d-168">A journal line can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="0223d-169">Uma conta (AccountId) deve existir na tabela accounts.</span><span class="sxs-lookup"><span data-stu-id="0223d-169">An Account (accountId) must exist in the Accounts table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0223d-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0223d-170">JSON representation</span></span>

<span data-ttu-id="0223d-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0223d-171">Here is a JSON representation of the resource.</span></span>


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
