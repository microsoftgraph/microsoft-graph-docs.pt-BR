---
title: Listar managedAppOperations
description: Listar propriedades e relações de objetos de managedAppOperation.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c7e5dc4fb67e511933fb6e5c355a4d6f0da4e4a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513172"
---
# <a name="list-managedappoperations"></a><span data-ttu-id="d8867-103">Listar managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="d8867-103">List managedAppOperations</span></span>

<span data-ttu-id="d8867-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8867-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8867-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8867-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8867-106">Listar propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="d8867-106">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8867-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8867-107">Prerequisites</span></span>
<span data-ttu-id="d8867-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8867-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8867-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8867-110">Permission type</span></span>|<span data-ttu-id="d8867-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8867-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8867-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8867-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8867-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8867-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d8867-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8867-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8867-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8867-115">Not supported.</span></span>|
|<span data-ttu-id="d8867-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8867-116">Application</span></span>|<span data-ttu-id="d8867-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8867-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8867-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8867-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="d8867-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8867-119">Request headers</span></span>
|<span data-ttu-id="d8867-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8867-120">Header</span></span>|<span data-ttu-id="d8867-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d8867-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8867-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8867-122">Authorization</span></span>|<span data-ttu-id="d8867-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8867-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8867-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8867-124">Accept</span></span>|<span data-ttu-id="d8867-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8867-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8867-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8867-126">Request body</span></span>
<span data-ttu-id="d8867-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8867-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8867-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8867-128">Response</span></span>
<span data-ttu-id="d8867-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppOperation](../resources/intune-mam-managedappoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8867-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8867-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8867-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8867-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8867-131">Request</span></span>
<span data-ttu-id="d8867-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8867-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

### <a name="response"></a><span data-ttu-id="d8867-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8867-133">Response</span></span>
<span data-ttu-id="d8867-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8867-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




