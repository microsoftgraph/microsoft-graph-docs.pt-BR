---
title: Lista iosVppAppAssignedLicenses
description: Lista as propriedades e os relacionamentos dos objetos iosVppAppAssignedLicense.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b02e35b7f0d2a6f64c2e1e891db6a6ae066be90b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883206"
---
# <a name="list-iosvppappassignedlicenses"></a><span data-ttu-id="4ec28-103">Lista iosVppAppAssignedLicenses</span><span class="sxs-lookup"><span data-stu-id="4ec28-103">List iosVppAppAssignedLicenses</span></span>

> <span data-ttu-id="4ec28-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4ec28-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ec28-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4ec28-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ec28-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4ec28-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ec28-107">Lista as propriedades e os relacionamentos dos objetos [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="4ec28-107">List properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ec28-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ec28-108">Prerequisites</span></span>
<span data-ttu-id="4ec28-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ec28-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ec28-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ec28-111">Permission type</span></span>|<span data-ttu-id="4ec28-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ec28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ec28-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ec28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ec28-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ec28-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4ec28-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ec28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ec28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ec28-116">Not supported.</span></span>|
|<span data-ttu-id="4ec28-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ec28-117">Application</span></span>|<span data-ttu-id="4ec28-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ec28-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ec28-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ec28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="4ec28-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec28-120">Request headers</span></span>
|<span data-ttu-id="4ec28-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ec28-121">Header</span></span>|<span data-ttu-id="4ec28-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4ec28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ec28-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ec28-123">Authorization</span></span>|<span data-ttu-id="4ec28-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ec28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ec28-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ec28-125">Accept</span></span>|<span data-ttu-id="4ec28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ec28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ec28-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec28-127">Request body</span></span>
<span data-ttu-id="4ec28-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ec28-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ec28-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ec28-129">Response</span></span>
<span data-ttu-id="4ec28-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ec28-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ec28-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ec28-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ec28-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec28-132">Request</span></span>
<span data-ttu-id="4ec28-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ec28-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="4ec28-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ec28-134">Response</span></span>
<span data-ttu-id="4ec28-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ec28-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
      "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





