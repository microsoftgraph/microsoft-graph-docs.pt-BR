---
title: Listar managedAppConfigurations
description: Listar propriedades e relações dos objetos managedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e47a07c28a1a8a135e04767e5e79046549694547
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018292"
---
# <a name="list-managedappconfigurations"></a><span data-ttu-id="0852b-103">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="0852b-103">List managedAppConfigurations</span></span>

> <span data-ttu-id="0852b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0852b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0852b-105">Listar propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0852b-105">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0852b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0852b-106">Prerequisites</span></span>
<span data-ttu-id="0852b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0852b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0852b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0852b-109">Permission type</span></span>|<span data-ttu-id="0852b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0852b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0852b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0852b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0852b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0852b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0852b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0852b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0852b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0852b-114">Not supported.</span></span>|
|<span data-ttu-id="0852b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0852b-115">Application</span></span>|<span data-ttu-id="0852b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0852b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0852b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0852b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="0852b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0852b-118">Request headers</span></span>
|<span data-ttu-id="0852b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0852b-119">Header</span></span>|<span data-ttu-id="0852b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0852b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0852b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0852b-121">Authorization</span></span>|<span data-ttu-id="0852b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0852b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0852b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0852b-123">Accept</span></span>|<span data-ttu-id="0852b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0852b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0852b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0852b-125">Request body</span></span>
<span data-ttu-id="0852b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0852b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0852b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0852b-127">Response</span></span>
<span data-ttu-id="0852b-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0852b-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0852b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0852b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0852b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0852b-130">Request</span></span>
<span data-ttu-id="0852b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0852b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="0852b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0852b-132">Response</span></span>
<span data-ttu-id="0852b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0852b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "2ed27cb5-7cb5-2ed2-b57c-d22eb57cd22e",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```



