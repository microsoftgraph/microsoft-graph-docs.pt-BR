---
title: Listar mobileAppAssignments
description: Listar propriedades e relações dos objetos mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c5dfe8a05adba6ee07c436ae484bd5df3be55dd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541903"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="b8643-103">Listar mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="b8643-103">List mobileAppAssignments</span></span>

> <span data-ttu-id="b8643-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8643-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8643-105">Listar propriedades e relações dos objetos [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b8643-105">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8643-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8643-106">Prerequisites</span></span>
<span data-ttu-id="b8643-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8643-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8643-109">Permission type</span></span>|<span data-ttu-id="b8643-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8643-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8643-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8643-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8643-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8643-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b8643-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8643-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8643-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8643-114">Not supported.</span></span>|
|<span data-ttu-id="b8643-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8643-115">Application</span></span>|<span data-ttu-id="b8643-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8643-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8643-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8643-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b8643-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8643-118">Request headers</span></span>
|<span data-ttu-id="b8643-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8643-119">Header</span></span>|<span data-ttu-id="b8643-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b8643-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8643-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8643-121">Authorization</span></span>|<span data-ttu-id="b8643-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8643-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8643-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8643-123">Accept</span></span>|<span data-ttu-id="b8643-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b8643-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8643-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8643-125">Request body</span></span>
<span data-ttu-id="b8643-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8643-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8643-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8643-127">Response</span></span>
<span data-ttu-id="b8643-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8643-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8643-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8643-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8643-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8643-130">Request</span></span>
<span data-ttu-id="b8643-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8643-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="b8643-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8643-132">Response</span></span>
<span data-ttu-id="b8643-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8643-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



