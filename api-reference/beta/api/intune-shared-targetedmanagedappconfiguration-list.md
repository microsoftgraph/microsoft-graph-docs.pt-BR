---
title: Listar targetedManagedAppConfigurations
description: Listar propriedades e relações dos objetos targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db44fd3bf9e2b0b6afe4a293e9824cf7fa2aa0af
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085616"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="094d8-103">Listar targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="094d8-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="094d8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="094d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="094d8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="094d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="094d8-106">Listar propriedades e relações dos objetos [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="094d8-106">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="094d8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="094d8-107">Prerequisites</span></span>
<span data-ttu-id="094d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="094d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="094d8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="094d8-110">Permission type</span></span>|<span data-ttu-id="094d8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="094d8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="094d8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="094d8-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="094d8-113">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="094d8-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="094d8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="094d8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="094d8-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="094d8-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="094d8-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="094d8-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="094d8-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="094d8-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="094d8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="094d8-118">Not supported.</span></span>|
|<span data-ttu-id="094d8-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="094d8-119">Application</span></span>||
| <span data-ttu-id="094d8-120">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="094d8-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="094d8-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="094d8-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="094d8-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="094d8-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="094d8-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="094d8-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="094d8-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="094d8-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="094d8-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="094d8-125">Request headers</span></span>
|<span data-ttu-id="094d8-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="094d8-126">Header</span></span>|<span data-ttu-id="094d8-127">Valor</span><span class="sxs-lookup"><span data-stu-id="094d8-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="094d8-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="094d8-128">Authorization</span></span>|<span data-ttu-id="094d8-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="094d8-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="094d8-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="094d8-130">Accept</span></span>|<span data-ttu-id="094d8-131">application/json</span><span class="sxs-lookup"><span data-stu-id="094d8-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="094d8-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="094d8-132">Request body</span></span>
<span data-ttu-id="094d8-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="094d8-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="094d8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="094d8-134">Response</span></span>
<span data-ttu-id="094d8-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="094d8-135">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="094d8-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="094d8-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="094d8-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="094d8-137">Request</span></span>
<span data-ttu-id="094d8-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="094d8-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="094d8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="094d8-139">Response</span></span>
<span data-ttu-id="094d8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="094d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 731

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "2444e029-e029-2444-29e0-442429e04424",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "isAssigned": true
    }
  ]
}
```









