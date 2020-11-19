---
title: Listar managedAppOperations
description: Listar propriedades e relações de objetos de managedAppOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f9ca7423b88aca4971c4e033855e9893bc916ee
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49277593"
---
# <a name="list-managedappoperations"></a><span data-ttu-id="8fc1e-103">Listar managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="8fc1e-103">List managedAppOperations</span></span>

<span data-ttu-id="8fc1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fc1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fc1e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8fc1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fc1e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8fc1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fc1e-107">Listar propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="8fc1e-107">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fc1e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8fc1e-108">Prerequisites</span></span>
<span data-ttu-id="8fc1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fc1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fc1e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fc1e-111">Permission type</span></span>|<span data-ttu-id="8fc1e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8fc1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fc1e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fc1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fc1e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fc1e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8fc1e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fc1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fc1e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fc1e-116">Not supported.</span></span>|
|<span data-ttu-id="8fc1e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fc1e-117">Application</span></span>|<span data-ttu-id="8fc1e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fc1e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fc1e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fc1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="8fc1e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fc1e-120">Request headers</span></span>
|<span data-ttu-id="8fc1e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8fc1e-121">Header</span></span>|<span data-ttu-id="8fc1e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8fc1e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fc1e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fc1e-123">Authorization</span></span>|<span data-ttu-id="8fc1e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fc1e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fc1e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8fc1e-125">Accept</span></span>|<span data-ttu-id="8fc1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fc1e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fc1e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fc1e-127">Request body</span></span>
<span data-ttu-id="8fc1e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8fc1e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fc1e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fc1e-129">Response</span></span>
<span data-ttu-id="8fc1e-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppOperation](../resources/intune-mam-managedappoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fc1e-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fc1e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fc1e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fc1e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fc1e-132">Request</span></span>
<span data-ttu-id="8fc1e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fc1e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

### <a name="response"></a><span data-ttu-id="8fc1e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fc1e-134">Response</span></span>
<span data-ttu-id="8fc1e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fc1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppOperation",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "State value",
      "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
      "version": "Version value"
    }
  ]
}
```




