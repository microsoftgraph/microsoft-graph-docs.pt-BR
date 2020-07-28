---
title: tipo de recurso educationSynchronizationError
description: Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 59650bc56554b9bd4dd7135ae44d53e153c159f8
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434834"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="33be7-103">tipo de recurso educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="33be7-103">educationSynchronizationError resource type</span></span>

<span data-ttu-id="33be7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33be7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33be7-105">Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="33be7-105">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="33be7-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="33be7-106">Methods</span></span>

| <span data-ttu-id="33be7-107">Método</span><span class="sxs-lookup"><span data-stu-id="33be7-107">Method</span></span>                                                                     | <span data-ttu-id="33be7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="33be7-108">Return Type</span></span>                                  | <span data-ttu-id="33be7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="33be7-109">Description</span></span>                                                           |
| :------------------------------------------------------------------------- | :------------------------------------------- | :-------------------------------------------------------------------- |
| [<span data-ttu-id="33be7-110">Obter erros de sincronização</span><span class="sxs-lookup"><span data-stu-id="33be7-110">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="33be7-111">coleção **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="33be7-111">**educationSynchronizationError** collection</span></span> | <span data-ttu-id="33be7-112">Retorna a lista de erros de sincronização associados a um perfil.</span><span class="sxs-lookup"><span data-stu-id="33be7-112">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="33be7-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33be7-113">Properties</span></span>

| <span data-ttu-id="33be7-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33be7-114">Property</span></span>             | <span data-ttu-id="33be7-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="33be7-115">Type</span></span>           | <span data-ttu-id="33be7-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="33be7-116">Description</span></span>                                                     |
| :------------------- | :------------- | :-------------------------------------------------------------- |
| <span data-ttu-id="33be7-117">id</span><span class="sxs-lookup"><span data-stu-id="33be7-117">id</span></span>                   | <span data-ttu-id="33be7-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33be7-118">String</span></span>         | <span data-ttu-id="33be7-119">O identificador exclusivo do recurso.</span><span class="sxs-lookup"><span data-stu-id="33be7-119">The unique identifier for the resource.</span></span> <span data-ttu-id="33be7-120">(somente leitura)</span><span class="sxs-lookup"><span data-stu-id="33be7-120">(read-only)</span></span>             |
| <span data-ttu-id="33be7-121">EntryType</span><span class="sxs-lookup"><span data-stu-id="33be7-121">entryType</span></span>            | <span data-ttu-id="33be7-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33be7-122">String</span></span>         | <span data-ttu-id="33be7-123">Representa a entidade de sincronização (escola, seção, aluno, professor).</span><span class="sxs-lookup"><span data-stu-id="33be7-123">Represents the sync entity (school, section, student, teacher).</span></span> |
| <span data-ttu-id="33be7-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="33be7-124">errorCode</span></span>            | <span data-ttu-id="33be7-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33be7-125">String</span></span>         | <span data-ttu-id="33be7-126">Representa o código de erro para esse erro.</span><span class="sxs-lookup"><span data-stu-id="33be7-126">Represents the error code for this error.</span></span>                       |
| <span data-ttu-id="33be7-127">errorMessage</span><span class="sxs-lookup"><span data-stu-id="33be7-127">errorMessage</span></span>         | <span data-ttu-id="33be7-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33be7-128">String</span></span>         | <span data-ttu-id="33be7-129">Contém uma descrição do erro.</span><span class="sxs-lookup"><span data-stu-id="33be7-129">Contains a description of the error.</span></span>                            |
| <span data-ttu-id="33be7-130">unindovalue</span><span class="sxs-lookup"><span data-stu-id="33be7-130">joiningValue</span></span>         | <span data-ttu-id="33be7-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33be7-131">String</span></span>         | <span data-ttu-id="33be7-132">O identificador exclusivo da entrada.</span><span class="sxs-lookup"><span data-stu-id="33be7-132">The unique identifier for the entry.</span></span>                            |
| <span data-ttu-id="33be7-133">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="33be7-133">recordedDateTime</span></span>     | <span data-ttu-id="33be7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33be7-134">DateTimeOffset</span></span> | <span data-ttu-id="33be7-135">A hora da ocorrência desse erro.</span><span class="sxs-lookup"><span data-stu-id="33be7-135">The time of occurrence of this error.</span></span>                           |
| <span data-ttu-id="33be7-136">reportableIdentifier</span><span class="sxs-lookup"><span data-stu-id="33be7-136">reportableIdentifier</span></span> | <span data-ttu-id="33be7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33be7-137">String</span></span>         | <span data-ttu-id="33be7-138">O identificador desta entrada de erro.</span><span class="sxs-lookup"><span data-stu-id="33be7-138">The identifier of this error entry.</span></span>                             |

## <a name="json-representation"></a><span data-ttu-id="33be7-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33be7-139">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
  "id": "String",
  "entryType": "String",
  "errorCode": "String",
  "errorMessage": "String",
  "joiningValue": "String",
  "recordedDateTime": "DateTimeOffset",
  "reportableIdentifier": "String"
}
```
