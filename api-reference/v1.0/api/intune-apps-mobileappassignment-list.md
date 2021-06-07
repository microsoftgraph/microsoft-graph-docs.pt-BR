---
title: Listar mobileAppAssignments
description: Listar propriedades e relações dos objetos mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 709466f2c758c365c8ebb353481bcd77ad08738a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754109"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="8e6ae-103">Listar mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="8e6ae-103">List mobileAppAssignments</span></span>

<span data-ttu-id="8e6ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e6ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e6ae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e6ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e6ae-106">Listar propriedades e relações dos objetos [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8e6ae-106">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e6ae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e6ae-107">Prerequisites</span></span>
<span data-ttu-id="8e6ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e6ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e6ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e6ae-110">Permission type</span></span>|<span data-ttu-id="8e6ae-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e6ae-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e6ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e6ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e6ae-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e6ae-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e6ae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e6ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e6ae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e6ae-115">Not supported.</span></span>|
|<span data-ttu-id="8e6ae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e6ae-116">Application</span></span>|<span data-ttu-id="8e6ae-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e6ae-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e6ae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e6ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8e6ae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e6ae-119">Request headers</span></span>
|<span data-ttu-id="8e6ae-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e6ae-120">Header</span></span>|<span data-ttu-id="8e6ae-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8e6ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e6ae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e6ae-122">Authorization</span></span>|<span data-ttu-id="8e6ae-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e6ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e6ae-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e6ae-124">Accept</span></span>|<span data-ttu-id="8e6ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e6ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e6ae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e6ae-126">Request body</span></span>
<span data-ttu-id="8e6ae-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e6ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e6ae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e6ae-128">Response</span></span>
<span data-ttu-id="8e6ae-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e6ae-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e6ae-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e6ae-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e6ae-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e6ae-131">Request</span></span>
<span data-ttu-id="8e6ae-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e6ae-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="8e6ae-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e6ae-133">Response</span></span>
<span data-ttu-id="8e6ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e6ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
        "vpnConfigurationId": "Vpn Configuration Id value"
      }
    }
  ]
}
```




