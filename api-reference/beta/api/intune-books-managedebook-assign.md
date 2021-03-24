---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80003f8b50213f44fb5f378b08d5a7b5e303049f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133133"
---
# <a name="assign-action"></a><span data-ttu-id="b3312-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="b3312-103">assign action</span></span>

<span data-ttu-id="b3312-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3312-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3312-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3312-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3312-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3312-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3312-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b3312-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3312-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3312-108">Prerequisites</span></span>
<span data-ttu-id="b3312-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3312-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3312-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3312-111">Permission type</span></span>|<span data-ttu-id="b3312-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3312-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3312-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3312-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3312-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3312-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3312-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3312-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3312-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3312-116">Not supported.</span></span>|
|<span data-ttu-id="b3312-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3312-117">Application</span></span>|<span data-ttu-id="b3312-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3312-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3312-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3312-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b3312-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3312-120">Request headers</span></span>
|<span data-ttu-id="b3312-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3312-121">Header</span></span>|<span data-ttu-id="b3312-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b3312-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3312-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3312-123">Authorization</span></span>|<span data-ttu-id="b3312-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3312-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3312-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3312-125">Accept</span></span>|<span data-ttu-id="b3312-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3312-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3312-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3312-127">Request body</span></span>
<span data-ttu-id="b3312-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b3312-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b3312-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b3312-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b3312-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3312-130">Property</span></span>|<span data-ttu-id="b3312-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3312-131">Type</span></span>|<span data-ttu-id="b3312-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3312-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3312-133">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="b3312-133">managedEBookAssignments</span></span>|<span data-ttu-id="b3312-134">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b3312-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="b3312-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b3312-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b3312-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3312-136">Response</span></span>
<span data-ttu-id="b3312-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b3312-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b3312-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3312-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3312-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3312-139">Request</span></span>
<span data-ttu-id="b3312-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3312-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b3312-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3312-141">Response</span></span>
<span data-ttu-id="b3312-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3312-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




