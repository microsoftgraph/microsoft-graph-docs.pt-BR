---
title: Get managedEBookAssignment
description: Ler propriedades e relações do objeto managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00515ebfdbfa4e1843ffc001d32023e3b44e259e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133084"
---
# <a name="get-managedebookassignment"></a><span data-ttu-id="292ca-103">Get managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="292ca-103">Get managedEBookAssignment</span></span>

<span data-ttu-id="292ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="292ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="292ca-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="292ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="292ca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="292ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="292ca-107">Ler propriedades e relações do objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="292ca-107">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="292ca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="292ca-108">Prerequisites</span></span>
<span data-ttu-id="292ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="292ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="292ca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="292ca-111">Permission type</span></span>|<span data-ttu-id="292ca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="292ca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="292ca-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="292ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="292ca-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="292ca-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="292ca-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="292ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="292ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="292ca-116">Not supported.</span></span>|
|<span data-ttu-id="292ca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="292ca-117">Application</span></span>|<span data-ttu-id="292ca-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="292ca-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="292ca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="292ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="292ca-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="292ca-120">Optional query parameters</span></span>
<span data-ttu-id="292ca-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="292ca-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="292ca-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="292ca-122">Request headers</span></span>
|<span data-ttu-id="292ca-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="292ca-123">Header</span></span>|<span data-ttu-id="292ca-124">Valor</span><span class="sxs-lookup"><span data-stu-id="292ca-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="292ca-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="292ca-125">Authorization</span></span>|<span data-ttu-id="292ca-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="292ca-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="292ca-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="292ca-127">Accept</span></span>|<span data-ttu-id="292ca-128">application/json</span><span class="sxs-lookup"><span data-stu-id="292ca-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="292ca-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="292ca-129">Request body</span></span>
<span data-ttu-id="292ca-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="292ca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="292ca-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="292ca-131">Response</span></span>
<span data-ttu-id="292ca-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="292ca-132">If successful, this method returns a `200 OK` response code and [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="292ca-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="292ca-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="292ca-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="292ca-134">Request</span></span>
<span data-ttu-id="292ca-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="292ca-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="292ca-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="292ca-136">Response</span></span>
<span data-ttu-id="292ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="292ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBookAssignment",
    "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
    "target": {
      "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    },
    "installIntent": "required"
  }
}
```




