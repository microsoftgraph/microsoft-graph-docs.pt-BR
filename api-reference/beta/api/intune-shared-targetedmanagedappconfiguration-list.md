---
title: Listar targetedManagedAppConfigurations
description: Listar propriedades e relações dos objetos targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 66962de7861d717ee73ba73c32acafa74fcfb753
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465305"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="2a603-103">Listar targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="2a603-103">List targetedManagedAppConfigurations</span></span>

<span data-ttu-id="2a603-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a603-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a603-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a603-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a603-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a603-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a603-107">Listar propriedades e relações dos objetos [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a603-107">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a603-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a603-108">Prerequisites</span></span>
<span data-ttu-id="2a603-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a603-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a603-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a603-111">Permission type</span></span>|<span data-ttu-id="2a603-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a603-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a603-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a603-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2a603-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="2a603-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="2a603-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a603-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="2a603-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="2a603-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2a603-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a603-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2a603-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a603-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a603-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a603-119">Not supported.</span></span>|
|<span data-ttu-id="2a603-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a603-120">Application</span></span>||
| <span data-ttu-id="2a603-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="2a603-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="2a603-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a603-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="2a603-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="2a603-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2a603-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a603-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a603-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a603-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2a603-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a603-126">Request headers</span></span>
|<span data-ttu-id="2a603-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a603-127">Header</span></span>|<span data-ttu-id="2a603-128">Valor</span><span class="sxs-lookup"><span data-stu-id="2a603-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a603-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a603-129">Authorization</span></span>|<span data-ttu-id="2a603-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a603-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a603-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a603-131">Accept</span></span>|<span data-ttu-id="2a603-132">application/json</span><span class="sxs-lookup"><span data-stu-id="2a603-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a603-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a603-133">Request body</span></span>
<span data-ttu-id="2a603-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a603-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a603-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a603-135">Response</span></span>
<span data-ttu-id="2a603-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a603-136">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a603-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a603-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a603-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a603-138">Request</span></span>
<span data-ttu-id="2a603-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a603-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="2a603-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a603-140">Response</span></span>
<span data-ttu-id="2a603-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a603-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






