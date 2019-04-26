---
title: Listar managedAppOperations
description: Listar propriedades e relações de objetos de managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3ae31a7077b5003cf6c88f15afc4d45d9dda9a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571048"
---
# <a name="list-managedappoperations"></a><span data-ttu-id="414a2-103">Listar managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="414a2-103">List managedAppOperations</span></span>

> <span data-ttu-id="414a2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="414a2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="414a2-105">Listar propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="414a2-105">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="414a2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="414a2-106">Prerequisites</span></span>
<span data-ttu-id="414a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="414a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="414a2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="414a2-109">Permission type</span></span>|<span data-ttu-id="414a2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="414a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="414a2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="414a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="414a2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="414a2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="414a2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="414a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="414a2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="414a2-114">Not supported.</span></span>|
|<span data-ttu-id="414a2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="414a2-115">Application</span></span>|<span data-ttu-id="414a2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="414a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="414a2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="414a2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="414a2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="414a2-118">Request headers</span></span>
|<span data-ttu-id="414a2-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="414a2-119">Header</span></span>|<span data-ttu-id="414a2-120">Valor</span><span class="sxs-lookup"><span data-stu-id="414a2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="414a2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="414a2-121">Authorization</span></span>|<span data-ttu-id="414a2-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="414a2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="414a2-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="414a2-123">Accept</span></span>|<span data-ttu-id="414a2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="414a2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="414a2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="414a2-125">Request body</span></span>
<span data-ttu-id="414a2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="414a2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="414a2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="414a2-127">Response</span></span>
<span data-ttu-id="414a2-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppOperation](../resources/intune-mam-managedappoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="414a2-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="414a2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="414a2-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="414a2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="414a2-130">Request</span></span>
<span data-ttu-id="414a2-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="414a2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

### <a name="response"></a><span data-ttu-id="414a2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="414a2-132">Response</span></span>
<span data-ttu-id="414a2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="414a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



