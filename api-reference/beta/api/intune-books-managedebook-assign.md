---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cbe825eae1ac6fe8d5af5cef347a30fe3340956b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793210"
---
# <a name="assign-action"></a><span data-ttu-id="abadb-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="abadb-103">assign action</span></span>

<span data-ttu-id="abadb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abadb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abadb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abadb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abadb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abadb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abadb-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="abadb-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abadb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abadb-108">Prerequisites</span></span>
<span data-ttu-id="abadb-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="abadb-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="abadb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abadb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abadb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abadb-111">Permission type</span></span>|<span data-ttu-id="abadb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abadb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abadb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abadb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abadb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abadb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="abadb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abadb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abadb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abadb-116">Not supported.</span></span>|
|<span data-ttu-id="abadb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abadb-117">Application</span></span>|<span data-ttu-id="abadb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abadb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abadb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abadb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="abadb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abadb-120">Request headers</span></span>
|<span data-ttu-id="abadb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abadb-121">Header</span></span>|<span data-ttu-id="abadb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="abadb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abadb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="abadb-123">Authorization</span></span>|<span data-ttu-id="abadb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abadb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abadb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abadb-125">Accept</span></span>|<span data-ttu-id="abadb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abadb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abadb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abadb-127">Request body</span></span>
<span data-ttu-id="abadb-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="abadb-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="abadb-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="abadb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="abadb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abadb-130">Property</span></span>|<span data-ttu-id="abadb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="abadb-131">Type</span></span>|<span data-ttu-id="abadb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="abadb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abadb-133">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="abadb-133">managedEBookAssignments</span></span>|<span data-ttu-id="abadb-134">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="abadb-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="abadb-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="abadb-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="abadb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="abadb-136">Response</span></span>
<span data-ttu-id="abadb-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="abadb-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="abadb-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abadb-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="abadb-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abadb-139">Request</span></span>
<span data-ttu-id="abadb-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abadb-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 487

{
  "managedEBookAssignments": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "installIntent": "required"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="abadb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="abadb-141">Response</span></span>
<span data-ttu-id="abadb-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="abadb-142">Here is an example of the response.</span></span> <span data-ttu-id="abadb-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="abadb-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="abadb-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="abadb-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



