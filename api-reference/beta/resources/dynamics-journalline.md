---
title: tipo de recurso journalLines
description: Uma linha de diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7a6841bcc2f893f8ca794e7d8e6aeafbcd4e48ca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507291"
---
# <a name="journallines-resource-type"></a><span data-ttu-id="1e4d1-103">tipo de recurso journalLines</span><span class="sxs-lookup"><span data-stu-id="1e4d1-103">journalLines resource type</span></span>
<span data-ttu-id="1e4d1-104">Representa uma linha em um diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-104">Represents a line in a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="1e4d1-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1e4d1-105">Methods</span></span>

| <span data-ttu-id="1e4d1-106">Método</span><span class="sxs-lookup"><span data-stu-id="1e4d1-106">Method</span></span>                                                    | <span data-ttu-id="1e4d1-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1e4d1-107">Return Type</span></span>|<span data-ttu-id="1e4d1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e4d1-108">Description</span></span>         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[<span data-ttu-id="1e4d1-109">Obter journalLines</span><span class="sxs-lookup"><span data-stu-id="1e4d1-109">Get journalLines</span></span>](../api/dynamics-journalline-get.md)      |<span data-ttu-id="1e4d1-110">journalLines</span><span class="sxs-lookup"><span data-stu-id="1e4d1-110">journalLines</span></span>|<span data-ttu-id="1e4d1-111">Obtém uma linha do diário.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-111">Gets a journal line.</span></span>   |
|[<span data-ttu-id="1e4d1-112">Postar journalLines</span><span class="sxs-lookup"><span data-stu-id="1e4d1-112">Post journalLines</span></span>](../api/dynamics-create-journalline.md)  |<span data-ttu-id="1e4d1-113">journalLines</span><span class="sxs-lookup"><span data-stu-id="1e4d1-113">journalLines</span></span>|<span data-ttu-id="1e4d1-114">Cria uma linha de diário.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-114">Creates a journal line.</span></span>|
|[<span data-ttu-id="1e4d1-115">Patch journalLines</span><span class="sxs-lookup"><span data-stu-id="1e4d1-115">Patch journalLines</span></span>](../api/dynamics-journalline-update.md) |<span data-ttu-id="1e4d1-116">journalLines</span><span class="sxs-lookup"><span data-stu-id="1e4d1-116">journalLines</span></span>|<span data-ttu-id="1e4d1-117">Atualiza uma linha do diário.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-117">Updates a journal line.</span></span>|
|[<span data-ttu-id="1e4d1-118">Excluir journalLines</span><span class="sxs-lookup"><span data-stu-id="1e4d1-118">Delete journalLines</span></span>](../api/dynamics-journalline-delete.md)|<span data-ttu-id="1e4d1-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1e4d1-119">none</span></span>        |<span data-ttu-id="1e4d1-120">Exclui uma linha do diário.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-120">Deletes a journal line.</span></span>|

## <a name="properties"></a><span data-ttu-id="1e4d1-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e4d1-121">Properties</span></span>
| <span data-ttu-id="1e4d1-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e4d1-122">Property</span></span>             | <span data-ttu-id="1e4d1-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e4d1-123">Type</span></span>                   |<span data-ttu-id="1e4d1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e4d1-124">Description</span></span>                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|<span data-ttu-id="1e4d1-125">id</span><span class="sxs-lookup"><span data-stu-id="1e4d1-125">id</span></span>                    |<span data-ttu-id="1e4d1-126">GUID</span><span class="sxs-lookup"><span data-stu-id="1e4d1-126">GUID</span></span>                    |<span data-ttu-id="1e4d1-127">A identificação exclusiva da linha do diário.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-127">The unique ID of the journal line.</span></span> <span data-ttu-id="1e4d1-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-128">Non-editable.</span></span>                   |
|<span data-ttu-id="1e4d1-129">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="1e4d1-129">journalDisplayName</span></span>    |<span data-ttu-id="1e4d1-130">Cadeia de caracteres, tamanho máximo 10</span><span class="sxs-lookup"><span data-stu-id="1e4d1-130">string, maximum size 10</span></span> |<span data-ttu-id="1e4d1-131">O nome de exibição do diário ao qual esta linha pertence.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-131">The display name of the journal that this line belongs to.</span></span> <span data-ttu-id="1e4d1-132">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-132">Read-Only.</span></span>|
|<span data-ttu-id="1e4d1-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="1e4d1-133">lineNumber</span></span>            |<span data-ttu-id="1e4d1-134">inteiro</span><span class="sxs-lookup"><span data-stu-id="1e4d1-134">integer</span></span>                 |<span data-ttu-id="1e4d1-135">O número da linha do diário.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-135">The number of the journal line.</span></span>                                    |
|<span data-ttu-id="1e4d1-136">accountId</span><span class="sxs-lookup"><span data-stu-id="1e4d1-136">accountId</span></span>             |<span data-ttu-id="1e4d1-137">GUID</span><span class="sxs-lookup"><span data-stu-id="1e4d1-137">GUID</span></span>                    |<span data-ttu-id="1e4d1-138">A identificação exclusiva da conta à qual a linha do diário está relacionada.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-138">The unique ID of the account that the journal line is related to.</span></span>  |
|<span data-ttu-id="1e4d1-139">accountNumber</span><span class="sxs-lookup"><span data-stu-id="1e4d1-139">accountNumber</span></span>         |<span data-ttu-id="1e4d1-140">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="1e4d1-140">string, maximum size 20</span></span> |<span data-ttu-id="1e4d1-141">O número da conta à qual a linha do diário está relacionada.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-141">The number of the account that the journal line is related to.</span></span>     |
|<span data-ttu-id="1e4d1-142">postingDate</span><span class="sxs-lookup"><span data-stu-id="1e4d1-142">postingDate</span></span>           |<span data-ttu-id="1e4d1-143">data</span><span class="sxs-lookup"><span data-stu-id="1e4d1-143">date</span></span>                    |<span data-ttu-id="1e4d1-144">A data em que a linha do diário é lançada.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-144">The date that the journal line is posted.</span></span>                          |
|<span data-ttu-id="1e4d1-145">documentNumber</span><span class="sxs-lookup"><span data-stu-id="1e4d1-145">documentNumber</span></span>        |<span data-ttu-id="1e4d1-146">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="1e4d1-146">string, maximum size 20</span></span> |<span data-ttu-id="1e4d1-147">Especifica um número de documento para a linha do diário.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-147">Specifies a document number for the journal line.</span></span>                  |
|<span data-ttu-id="1e4d1-148">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="1e4d1-148">externalDocumentNumber</span></span>|<span data-ttu-id="1e4d1-149">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="1e4d1-149">string, maximum size 20</span></span> |<span data-ttu-id="1e4d1-150">Especifica um número de documento externo para a linha do diário.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-150">Specifies an external document number for the journal line.</span></span>        |
|<span data-ttu-id="1e4d1-151">quantia</span><span class="sxs-lookup"><span data-stu-id="1e4d1-151">amount</span></span>                |<span data-ttu-id="1e4d1-152">dígitos</span><span class="sxs-lookup"><span data-stu-id="1e4d1-152">decimal</span></span>                 |<span data-ttu-id="1e4d1-153">Especifica o valor total (incluindo o IVA) que a linha do diário consiste.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-153">Specifies the total amount (including VAT) that the journal line consists of.</span></span>|
|<span data-ttu-id="1e4d1-154">description</span><span class="sxs-lookup"><span data-stu-id="1e4d1-154">description</span></span>           |<span data-ttu-id="1e4d1-155">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="1e4d1-155">string, maximum size 50</span></span> |<span data-ttu-id="1e4d1-156">A descrição da linha do diário, fornecida pelo usuário ou autocriada.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-156">The description of the journal line, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="1e4d1-157">comment</span><span class="sxs-lookup"><span data-stu-id="1e4d1-157">comment</span></span>               |<span data-ttu-id="1e4d1-158">Cadeia de caracteres, tamanho máximo 250</span><span class="sxs-lookup"><span data-stu-id="1e4d1-158">string, maximum size 250</span></span>|<span data-ttu-id="1e4d1-159">Um comentário especificado pelo usuário na linha do diário.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-159">A user specified comment on the journal line.</span></span>                      |
|<span data-ttu-id="1e4d1-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e4d1-160">lastModifiedDateTime</span></span>  |<span data-ttu-id="1e4d1-161">DateTime</span><span class="sxs-lookup"><span data-stu-id="1e4d1-161">datetime</span></span>                |<span data-ttu-id="1e4d1-162">O último DateTime em que a linha do diário foi modificada.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-162">The last datetime the journal line was modified.</span></span> <span data-ttu-id="1e4d1-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-163">Read-Only.</span></span>        |

## <a name="relationships"></a><span data-ttu-id="1e4d1-164">Relações</span><span class="sxs-lookup"><span data-stu-id="1e4d1-164">Relationships</span></span>
<span data-ttu-id="1e4d1-165">Uma linha de diário é uma subpágina de um diário.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-165">A journal line is a subpage of a journal.</span></span> <span data-ttu-id="1e4d1-166">Ele não pode ser acessado diretamente.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-166">It cannot be accessed directly.</span></span>

<span data-ttu-id="1e4d1-167">Uma linha de diário pode ser uma "entidade pai" das linhas de dimensão.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-167">A journal line can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="1e4d1-168">Uma conta (AccountId) deve existir na tabela acCounts.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-168">An Account (accountId) must exist in the Accounts table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="1e4d1-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e4d1-169">JSON representation</span></span>

<span data-ttu-id="1e4d1-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e4d1-170">Here is a JSON representation of the resource.</span></span>


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
