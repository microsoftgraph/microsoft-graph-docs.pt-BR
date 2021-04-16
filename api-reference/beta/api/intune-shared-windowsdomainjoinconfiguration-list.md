---
title: Listar windowsDomainJoinConfigurations
description: Listar propriedades e relações dos objetos windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ec04c4917f700688dc46445d754bbcfcda12121
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866598"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="3eebd-103">Listar windowsDomainJoinConfigurations</span><span class="sxs-lookup"><span data-stu-id="3eebd-103">List windowsDomainJoinConfigurations</span></span>

<span data-ttu-id="3eebd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eebd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3eebd-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3eebd-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3eebd-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3eebd-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3eebd-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3eebd-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eebd-108">Listar propriedades e relações dos [objetos windowsDomainJoinConfiguration.](../resources/intune-shared-windowsdomainjoinconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eebd-108">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3eebd-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3eebd-109">Prerequisites</span></span>
<span data-ttu-id="3eebd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eebd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eebd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3eebd-112">Permission type</span></span>|<span data-ttu-id="3eebd-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3eebd-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eebd-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3eebd-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3eebd-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3eebd-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3eebd-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3eebd-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3eebd-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3eebd-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eebd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eebd-118">Not supported.</span></span>|
|<span data-ttu-id="3eebd-119">Application</span><span class="sxs-lookup"><span data-stu-id="3eebd-119">Application</span></span>||
| <span data-ttu-id="3eebd-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3eebd-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3eebd-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3eebd-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eebd-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3eebd-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3eebd-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3eebd-123">Request headers</span></span>
|<span data-ttu-id="3eebd-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3eebd-124">Header</span></span>|<span data-ttu-id="3eebd-125">Valor</span><span class="sxs-lookup"><span data-stu-id="3eebd-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eebd-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3eebd-126">Authorization</span></span>|<span data-ttu-id="3eebd-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3eebd-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eebd-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3eebd-128">Accept</span></span>|<span data-ttu-id="3eebd-129">application/json</span><span class="sxs-lookup"><span data-stu-id="3eebd-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eebd-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3eebd-130">Request body</span></span>
<span data-ttu-id="3eebd-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3eebd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eebd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eebd-132">Response</span></span>
<span data-ttu-id="3eebd-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3eebd-133">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eebd-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3eebd-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="3eebd-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3eebd-135">Request</span></span>
<span data-ttu-id="3eebd-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3eebd-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3eebd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eebd-137">Response</span></span>
<span data-ttu-id="3eebd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3eebd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 760

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
      "id": "40118d08-8d08-4011-088d-1140088d1140",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "computerNameStaticPrefix": "Computer Name Static Prefix value",
      "computerNameSuffixRandomCharCount": 1,
      "activeDirectoryDomainName": "Active Directory Domain Name value",
      "organizationalUnit": "Organizational Unit value"
    }
  ]
}
```










