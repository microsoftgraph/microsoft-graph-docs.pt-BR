---
title: Listar mobileAppAssignments
description: Listar propriedades e relações dos objetos mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbc50a8bdf27aad35a9a846a8b9e13775ebb3376
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255672"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="efaf4-103">Listar mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="efaf4-103">List mobileAppAssignments</span></span>

> <span data-ttu-id="efaf4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="efaf4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efaf4-105">Listar propriedades e relações dos objetos [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="efaf4-105">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efaf4-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efaf4-106">Prerequisites</span></span>
<span data-ttu-id="efaf4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="efaf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="efaf4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efaf4-109">Permission type</span></span>|<span data-ttu-id="efaf4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="efaf4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efaf4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efaf4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="efaf4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="efaf4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="efaf4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efaf4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efaf4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efaf4-114">Not supported.</span></span>|
|<span data-ttu-id="efaf4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efaf4-115">Application</span></span>|<span data-ttu-id="efaf4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efaf4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efaf4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efaf4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="efaf4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efaf4-118">Request headers</span></span>
|<span data-ttu-id="efaf4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efaf4-119">Header</span></span>|<span data-ttu-id="efaf4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="efaf4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efaf4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="efaf4-121">Authorization</span></span>|<span data-ttu-id="efaf4-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efaf4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efaf4-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="efaf4-123">Accept</span></span>|<span data-ttu-id="efaf4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="efaf4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efaf4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efaf4-125">Request body</span></span>
<span data-ttu-id="efaf4-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="efaf4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efaf4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="efaf4-127">Response</span></span>
<span data-ttu-id="efaf4-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efaf4-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efaf4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efaf4-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="efaf4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efaf4-130">Request</span></span>
<span data-ttu-id="efaf4-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efaf4-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="efaf4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="efaf4-132">Response</span></span>
<span data-ttu-id="efaf4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efaf4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```



