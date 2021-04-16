---
title: Listar targetedManagedAppConfigurations
description: Listar propriedades e relações dos objetos targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56aa751eafe45534055bc661640d1781818f95c4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864568"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="c13f5-103">Listar targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="c13f5-103">List targetedManagedAppConfigurations</span></span>

<span data-ttu-id="c13f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c13f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c13f5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c13f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c13f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c13f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c13f5-107">Listar propriedades e relações dos objetos [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c13f5-107">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c13f5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c13f5-108">Prerequisites</span></span>
<span data-ttu-id="c13f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c13f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c13f5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c13f5-111">Permission type</span></span>|<span data-ttu-id="c13f5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c13f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c13f5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c13f5-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c13f5-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="c13f5-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c13f5-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c13f5-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c13f5-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="c13f5-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c13f5-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c13f5-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c13f5-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c13f5-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c13f5-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c13f5-119">Not supported.</span></span>|
|<span data-ttu-id="c13f5-120">Application</span><span class="sxs-lookup"><span data-stu-id="c13f5-120">Application</span></span>||
| <span data-ttu-id="c13f5-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="c13f5-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c13f5-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c13f5-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c13f5-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="c13f5-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c13f5-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c13f5-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c13f5-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c13f5-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c13f5-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c13f5-126">Request headers</span></span>
|<span data-ttu-id="c13f5-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c13f5-127">Header</span></span>|<span data-ttu-id="c13f5-128">Valor</span><span class="sxs-lookup"><span data-stu-id="c13f5-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c13f5-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="c13f5-129">Authorization</span></span>|<span data-ttu-id="c13f5-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c13f5-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c13f5-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c13f5-131">Accept</span></span>|<span data-ttu-id="c13f5-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c13f5-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c13f5-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c13f5-133">Request body</span></span>
<span data-ttu-id="c13f5-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c13f5-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c13f5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13f5-135">Response</span></span>
<span data-ttu-id="c13f5-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c13f5-136">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c13f5-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c13f5-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c13f5-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13f5-138">Request</span></span>
<span data-ttu-id="c13f5-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c13f5-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="c13f5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13f5-140">Response</span></span>
<span data-ttu-id="c13f5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c13f5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







