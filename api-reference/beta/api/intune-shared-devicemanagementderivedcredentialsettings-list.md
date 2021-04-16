---
title: Listar deviceManagementDerivedCredentialSettingses
description: Listar propriedades e relações dos objetos deviceManagementDerivedCredentialSettings.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 806cb2a4eb3844f9d9f279b45d00cf23114bbbc6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867858"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a><span data-ttu-id="a3bac-103">Listar deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="a3bac-103">List deviceManagementDerivedCredentialSettingses</span></span>

<span data-ttu-id="a3bac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3bac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3bac-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a3bac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3bac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3bac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3bac-107">Listar propriedades e relações dos [objetos deviceManagementDerivedCredentialSettings.](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a3bac-107">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3bac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3bac-108">Prerequisites</span></span>
<span data-ttu-id="a3bac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3bac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3bac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3bac-111">Permission type</span></span>|<span data-ttu-id="a3bac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a3bac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3bac-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3bac-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="a3bac-114">&nbsp;&nbsp; **Política de Acesso a Recursos**</span><span class="sxs-lookup"><span data-stu-id="a3bac-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="a3bac-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3bac-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a3bac-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3bac-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3bac-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3bac-117">Not supported.</span></span>|
|<span data-ttu-id="a3bac-118">Application</span><span class="sxs-lookup"><span data-stu-id="a3bac-118">Application</span></span>||
|<span data-ttu-id="a3bac-119">&nbsp;&nbsp; **Política de Acesso a Recursos**</span><span class="sxs-lookup"><span data-stu-id="a3bac-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="a3bac-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3bac-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3bac-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3bac-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="a3bac-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3bac-122">Request headers</span></span>
|<span data-ttu-id="a3bac-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3bac-123">Header</span></span>|<span data-ttu-id="a3bac-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a3bac-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3bac-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3bac-125">Authorization</span></span>|<span data-ttu-id="a3bac-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3bac-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3bac-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a3bac-127">Accept</span></span>|<span data-ttu-id="a3bac-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a3bac-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3bac-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3bac-129">Request body</span></span>
<span data-ttu-id="a3bac-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3bac-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3bac-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3bac-131">Response</span></span>
<span data-ttu-id="a3bac-132">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3bac-132">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3bac-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3bac-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3bac-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3bac-134">Request</span></span>
<span data-ttu-id="a3bac-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3bac-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a><span data-ttu-id="a3bac-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3bac-136">Response</span></span>
<span data-ttu-id="a3bac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3bac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








