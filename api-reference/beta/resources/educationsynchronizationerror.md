---
title: tipo de recurso educationSynchronizationError
description: Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542918"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="0a30a-103">tipo de recurso educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="0a30a-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a30a-104">Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0a30a-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="0a30a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0a30a-105">Methods</span></span>

| <span data-ttu-id="0a30a-106">Método</span><span class="sxs-lookup"><span data-stu-id="0a30a-106">Method</span></span> | <span data-ttu-id="0a30a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0a30a-107">Return Type</span></span> | <span data-ttu-id="0a30a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a30a-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="0a30a-109">Obter erros de sincronização</span><span class="sxs-lookup"><span data-stu-id="0a30a-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="0a30a-110">coleção **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="0a30a-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="0a30a-111">Retorna a lista de erros de sincronização associados a um perfil.</span><span class="sxs-lookup"><span data-stu-id="0a30a-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="0a30a-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a30a-112">Properties</span></span>

| <span data-ttu-id="0a30a-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a30a-113">Property</span></span> | <span data-ttu-id="0a30a-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a30a-114">Type</span></span> | <span data-ttu-id="0a30a-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a30a-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="0a30a-116">**EntryType**</span><span class="sxs-lookup"><span data-stu-id="0a30a-116">**entryType**</span></span> | <span data-ttu-id="0a30a-117">string</span><span class="sxs-lookup"><span data-stu-id="0a30a-117">string</span></span> |  <span data-ttu-id="0a30a-118">Representa a entidade de sincronização (escola, seção, aluno, professor).</span><span class="sxs-lookup"><span data-stu-id="0a30a-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="0a30a-119">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="0a30a-119">**errorCode**</span></span> | <span data-ttu-id="0a30a-120">string</span><span class="sxs-lookup"><span data-stu-id="0a30a-120">string</span></span> |  <span data-ttu-id="0a30a-121">Representa o código de erro para esse erro.</span><span class="sxs-lookup"><span data-stu-id="0a30a-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="0a30a-122">**errorMessage**</span><span class="sxs-lookup"><span data-stu-id="0a30a-122">**errorMessage**</span></span> | <span data-ttu-id="0a30a-123">string</span><span class="sxs-lookup"><span data-stu-id="0a30a-123">string</span></span> |  <span data-ttu-id="0a30a-124">Contém uma descrição do erro.</span><span class="sxs-lookup"><span data-stu-id="0a30a-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="0a30a-125">**unindovalue**</span><span class="sxs-lookup"><span data-stu-id="0a30a-125">**joiningValue**</span></span> | <span data-ttu-id="0a30a-126">string</span><span class="sxs-lookup"><span data-stu-id="0a30a-126">string</span></span> |  <span data-ttu-id="0a30a-127">O identificador exclusivo da entrada.</span><span class="sxs-lookup"><span data-stu-id="0a30a-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="0a30a-128">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="0a30a-128">**recordedDateTime**</span></span> | <span data-ttu-id="0a30a-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a30a-129">DateTimeOffset</span></span> | <span data-ttu-id="0a30a-130">A hora da ocorrência desse erro.</span><span class="sxs-lookup"><span data-stu-id="0a30a-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="0a30a-131">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="0a30a-131">**reportableIdentifier**</span></span> | <span data-ttu-id="0a30a-132">string</span><span class="sxs-lookup"><span data-stu-id="0a30a-132">string</span></span> | <span data-ttu-id="0a30a-133">O identificador desta entrada de erro.</span><span class="sxs-lookup"><span data-stu-id="0a30a-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="0a30a-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a30a-134">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
