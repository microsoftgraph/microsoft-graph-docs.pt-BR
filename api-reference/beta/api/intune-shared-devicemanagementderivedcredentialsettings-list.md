---
title: Listar deviceManagementDerivedCredentialSettingses
description: Listar Propriedades e relações dos objetos deviceManagementDerivedCredentialSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a7df05062988c9282d5dc5a7d103446971826e5
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086001"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a><span data-ttu-id="28563-103">Listar deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="28563-103">List deviceManagementDerivedCredentialSettingses</span></span>

> <span data-ttu-id="28563-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28563-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28563-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28563-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28563-106">Listar Propriedades e relações dos objetos [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="28563-106">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28563-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28563-107">Prerequisites</span></span>
<span data-ttu-id="28563-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28563-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28563-110">Permission type</span></span>|<span data-ttu-id="28563-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="28563-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28563-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28563-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="28563-113">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="28563-113">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="28563-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="28563-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="28563-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28563-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28563-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28563-116">Not supported.</span></span>|
|<span data-ttu-id="28563-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28563-117">Application</span></span>||
|<span data-ttu-id="28563-118">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="28563-118">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="28563-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="28563-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28563-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28563-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="28563-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28563-121">Request headers</span></span>
|<span data-ttu-id="28563-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28563-122">Header</span></span>|<span data-ttu-id="28563-123">Valor</span><span class="sxs-lookup"><span data-stu-id="28563-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28563-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="28563-124">Authorization</span></span>|<span data-ttu-id="28563-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28563-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28563-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28563-126">Accept</span></span>|<span data-ttu-id="28563-127">application/json</span><span class="sxs-lookup"><span data-stu-id="28563-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28563-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28563-128">Request body</span></span>
<span data-ttu-id="28563-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28563-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28563-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="28563-130">Response</span></span>
<span data-ttu-id="28563-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28563-131">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28563-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28563-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="28563-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28563-133">Request</span></span>
<span data-ttu-id="28563-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28563-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a><span data-ttu-id="28563-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="28563-135">Response</span></span>
<span data-ttu-id="28563-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28563-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 347

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
      "id": "bc650741-0741-bc65-4107-65bc410765bc",
      "helpUrl": "https://example.com/helpUrl/",
      "displayName": "Display Name value",
      "issuer": "entrustDatacard",
      "notificationType": "companyPortal"
    }
  ]
}
```










