---
title: tipo de recurso educationSynchronizationError
description: Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3c512f921e77468bb30e5109eec29afa9b395b7e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340507"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="d9623-103">tipo de recurso educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="d9623-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9623-104">Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d9623-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="d9623-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="d9623-105">Methods</span></span>

| <span data-ttu-id="d9623-106">Método</span><span class="sxs-lookup"><span data-stu-id="d9623-106">Method</span></span> | <span data-ttu-id="d9623-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d9623-107">Return Type</span></span> | <span data-ttu-id="d9623-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9623-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="d9623-109">Obter erros de sincronização</span><span class="sxs-lookup"><span data-stu-id="d9623-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="d9623-110">coleção **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="d9623-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="d9623-111">Retorna a lista de erros de sincronização associados a um perfil.</span><span class="sxs-lookup"><span data-stu-id="d9623-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="d9623-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9623-112">Properties</span></span>

| <span data-ttu-id="d9623-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9623-113">Property</span></span> | <span data-ttu-id="d9623-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9623-114">Type</span></span> | <span data-ttu-id="d9623-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9623-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d9623-116">**EntryType**</span><span class="sxs-lookup"><span data-stu-id="d9623-116">**entryType**</span></span> | <span data-ttu-id="d9623-117">string</span><span class="sxs-lookup"><span data-stu-id="d9623-117">string</span></span> |  <span data-ttu-id="d9623-118">Representa a entidade de sincronização (escola, seção, aluno, professor).</span><span class="sxs-lookup"><span data-stu-id="d9623-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="d9623-119">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="d9623-119">**errorCode**</span></span> | <span data-ttu-id="d9623-120">string</span><span class="sxs-lookup"><span data-stu-id="d9623-120">string</span></span> |  <span data-ttu-id="d9623-121">Representa o código de erro para esse erro.</span><span class="sxs-lookup"><span data-stu-id="d9623-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="d9623-122">**errorMessage**</span><span class="sxs-lookup"><span data-stu-id="d9623-122">**errorMessage**</span></span> | <span data-ttu-id="d9623-123">string</span><span class="sxs-lookup"><span data-stu-id="d9623-123">string</span></span> |  <span data-ttu-id="d9623-124">Contém uma descrição do erro.</span><span class="sxs-lookup"><span data-stu-id="d9623-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="d9623-125">**unindovalue**</span><span class="sxs-lookup"><span data-stu-id="d9623-125">**joiningValue**</span></span> | <span data-ttu-id="d9623-126">string</span><span class="sxs-lookup"><span data-stu-id="d9623-126">string</span></span> |  <span data-ttu-id="d9623-127">O identificador exclusivo da entrada.</span><span class="sxs-lookup"><span data-stu-id="d9623-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="d9623-128">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="d9623-128">**recordedDateTime**</span></span> | <span data-ttu-id="d9623-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9623-129">DateTimeOffset</span></span> | <span data-ttu-id="d9623-130">A hora da ocorrência desse erro.</span><span class="sxs-lookup"><span data-stu-id="d9623-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="d9623-131">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="d9623-131">**reportableIdentifier**</span></span> | <span data-ttu-id="d9623-132">string</span><span class="sxs-lookup"><span data-stu-id="d9623-132">string</span></span> | <span data-ttu-id="d9623-133">O identificador desta entrada de erro.</span><span class="sxs-lookup"><span data-stu-id="d9623-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="d9623-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9623-134">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
