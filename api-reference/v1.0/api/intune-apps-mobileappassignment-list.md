---
title: Listar mobileAppAssignments
description: Listar propriedades e relações dos objetos mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e44cc08163094a9d13b1018369665a47cfd9bf79
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464891"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="64b30-103">Listar mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="64b30-103">List mobileAppAssignments</span></span>

<span data-ttu-id="64b30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64b30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64b30-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64b30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64b30-106">Listar propriedades e relações dos objetos [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="64b30-106">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64b30-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64b30-107">Prerequisites</span></span>
<span data-ttu-id="64b30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64b30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64b30-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64b30-110">Permission type</span></span>|<span data-ttu-id="64b30-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64b30-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64b30-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64b30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64b30-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64b30-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="64b30-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64b30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64b30-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64b30-115">Not supported.</span></span>|
|<span data-ttu-id="64b30-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64b30-116">Application</span></span>|<span data-ttu-id="64b30-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64b30-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64b30-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64b30-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="64b30-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64b30-119">Request headers</span></span>
|<span data-ttu-id="64b30-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64b30-120">Header</span></span>|<span data-ttu-id="64b30-121">Valor</span><span class="sxs-lookup"><span data-stu-id="64b30-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64b30-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="64b30-122">Authorization</span></span>|<span data-ttu-id="64b30-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64b30-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64b30-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64b30-124">Accept</span></span>|<span data-ttu-id="64b30-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64b30-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64b30-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64b30-126">Request body</span></span>
<span data-ttu-id="64b30-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64b30-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64b30-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b30-128">Response</span></span>
<span data-ttu-id="64b30-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64b30-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64b30-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64b30-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="64b30-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64b30-131">Request</span></span>
<span data-ttu-id="64b30-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64b30-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="64b30-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b30-133">Response</span></span>
<span data-ttu-id="64b30-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64b30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






