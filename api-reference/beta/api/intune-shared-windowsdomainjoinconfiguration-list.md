---
title: Listar windowsDomainJoinConfigurations
description: Listar Propriedades e relações dos objetos windowsDomainJoinConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a7311e9d3ed98a3cb4f45e8cc99c0d86777be171
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447325"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="9e460-103">Listar windowsDomainJoinConfigurations</span><span class="sxs-lookup"><span data-stu-id="9e460-103">List windowsDomainJoinConfigurations</span></span>

<span data-ttu-id="9e460-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e460-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e460-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9e460-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9e460-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9e460-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e460-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e460-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e460-108">Listar Propriedades e relações dos objetos [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9e460-108">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e460-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e460-109">Prerequisites</span></span>
<span data-ttu-id="9e460-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e460-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e460-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e460-112">Permission type</span></span>|<span data-ttu-id="9e460-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e460-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e460-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e460-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9e460-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="9e460-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="9e460-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e460-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9e460-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e460-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e460-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e460-118">Not supported.</span></span>|
|<span data-ttu-id="9e460-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e460-119">Application</span></span>||
| <span data-ttu-id="9e460-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="9e460-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="9e460-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e460-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e460-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e460-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9e460-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e460-123">Request headers</span></span>
|<span data-ttu-id="9e460-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e460-124">Header</span></span>|<span data-ttu-id="9e460-125">Valor</span><span class="sxs-lookup"><span data-stu-id="9e460-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e460-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e460-126">Authorization</span></span>|<span data-ttu-id="9e460-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e460-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e460-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e460-128">Accept</span></span>|<span data-ttu-id="9e460-129">application/json</span><span class="sxs-lookup"><span data-stu-id="9e460-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e460-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e460-130">Request body</span></span>
<span data-ttu-id="9e460-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e460-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e460-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e460-132">Response</span></span>
<span data-ttu-id="9e460-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e460-133">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e460-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e460-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e460-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e460-135">Request</span></span>
<span data-ttu-id="9e460-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e460-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9e460-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e460-137">Response</span></span>
<span data-ttu-id="9e460-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e460-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









