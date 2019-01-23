---
title: Lista macOsVppAppAssignedLicenses
description: Lista as propriedades e os relacionamentos dos objetos macOsVppAppAssignedLicense.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c6bf22365acec788d22dbf7893d2e1d85bebd852
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429154"
---
# <a name="list-macosvppappassignedlicenses"></a><span data-ttu-id="4edcb-103">Lista macOsVppAppAssignedLicenses</span><span class="sxs-lookup"><span data-stu-id="4edcb-103">List macOsVppAppAssignedLicenses</span></span>

> <span data-ttu-id="4edcb-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4edcb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4edcb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4edcb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4edcb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4edcb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4edcb-107">Lista as propriedades e os relacionamentos dos objetos [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="4edcb-107">List properties and relationships of the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4edcb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4edcb-108">Prerequisites</span></span>
<span data-ttu-id="4edcb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4edcb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4edcb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4edcb-111">Permission type</span></span>|<span data-ttu-id="4edcb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4edcb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4edcb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4edcb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4edcb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4edcb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4edcb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4edcb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4edcb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4edcb-116">Not supported.</span></span>|
|<span data-ttu-id="4edcb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4edcb-117">Application</span></span>|<span data-ttu-id="4edcb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4edcb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4edcb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4edcb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="4edcb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4edcb-120">Request headers</span></span>
|<span data-ttu-id="4edcb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4edcb-121">Header</span></span>|<span data-ttu-id="4edcb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4edcb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4edcb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4edcb-123">Authorization</span></span>|<span data-ttu-id="4edcb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4edcb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4edcb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4edcb-125">Accept</span></span>|<span data-ttu-id="4edcb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4edcb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4edcb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4edcb-127">Request body</span></span>
<span data-ttu-id="4edcb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4edcb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4edcb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4edcb-129">Response</span></span>
<span data-ttu-id="4edcb-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4edcb-130">If successful, this method returns a `200 OK` response code and a collection of [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4edcb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4edcb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4edcb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4edcb-132">Request</span></span>
<span data-ttu-id="4edcb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4edcb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="4edcb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4edcb-134">Response</span></span>
<span data-ttu-id="4edcb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4edcb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
      "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




