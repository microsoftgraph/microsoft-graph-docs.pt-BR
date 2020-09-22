---
title: Listar deviceManagementDerivedCredentialSettingses
description: Listar Propriedades e relações dos objetos deviceManagementDerivedCredentialSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0cfde9df41c52b8f31d318d424865e49a59898b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074395"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a><span data-ttu-id="ad8a2-103">Listar deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="ad8a2-103">List deviceManagementDerivedCredentialSettingses</span></span>

<span data-ttu-id="ad8a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad8a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad8a2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ad8a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad8a2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ad8a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad8a2-107">Listar Propriedades e relações dos objetos [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="ad8a2-107">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad8a2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad8a2-108">Prerequisites</span></span>
<span data-ttu-id="ad8a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad8a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad8a2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad8a2-111">Permission type</span></span>|<span data-ttu-id="ad8a2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad8a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad8a2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad8a2-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="ad8a2-114">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="ad8a2-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="ad8a2-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad8a2-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ad8a2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad8a2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad8a2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad8a2-117">Not supported.</span></span>|
|<span data-ttu-id="ad8a2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad8a2-118">Application</span></span>||
|<span data-ttu-id="ad8a2-119">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="ad8a2-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="ad8a2-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad8a2-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad8a2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad8a2-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="ad8a2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad8a2-122">Request headers</span></span>
|<span data-ttu-id="ad8a2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad8a2-123">Header</span></span>|<span data-ttu-id="ad8a2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ad8a2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad8a2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad8a2-125">Authorization</span></span>|<span data-ttu-id="ad8a2-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad8a2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad8a2-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ad8a2-127">Accept</span></span>|<span data-ttu-id="ad8a2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ad8a2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad8a2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad8a2-129">Request body</span></span>
<span data-ttu-id="ad8a2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad8a2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad8a2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad8a2-131">Response</span></span>
<span data-ttu-id="ad8a2-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad8a2-132">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad8a2-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad8a2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad8a2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad8a2-134">Request</span></span>
<span data-ttu-id="ad8a2-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad8a2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a><span data-ttu-id="ad8a2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad8a2-136">Response</span></span>
<span data-ttu-id="ad8a2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad8a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










