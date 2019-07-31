---
title: Listar windowsDomainJoinConfigurations
description: Listar Propriedades e relações dos objetos windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d692837bd48d2b7dcbe23634ae590f79786c71e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993519"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="6182e-103">Listar windowsDomainJoinConfigurations</span><span class="sxs-lookup"><span data-stu-id="6182e-103">List windowsDomainJoinConfigurations</span></span>

> <span data-ttu-id="6182e-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6182e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6182e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6182e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6182e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6182e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6182e-107">Listar Propriedades e relações dos objetos [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6182e-107">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6182e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6182e-108">Prerequisites</span></span>
<span data-ttu-id="6182e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6182e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6182e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6182e-111">Permission type</span></span>|<span data-ttu-id="6182e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6182e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6182e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6182e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6182e-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="6182e-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6182e-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6182e-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6182e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6182e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6182e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6182e-117">Not supported.</span></span>|
|<span data-ttu-id="6182e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6182e-118">Application</span></span>|<span data-ttu-id="6182e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6182e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6182e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6182e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6182e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6182e-121">Request headers</span></span>
|<span data-ttu-id="6182e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6182e-122">Header</span></span>|<span data-ttu-id="6182e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6182e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6182e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6182e-124">Authorization</span></span>|<span data-ttu-id="6182e-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6182e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6182e-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6182e-126">Accept</span></span>|<span data-ttu-id="6182e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6182e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6182e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6182e-128">Request body</span></span>
<span data-ttu-id="6182e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6182e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6182e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6182e-130">Response</span></span>
<span data-ttu-id="6182e-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6182e-131">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6182e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6182e-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="6182e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6182e-133">Request</span></span>
<span data-ttu-id="6182e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6182e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6182e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6182e-135">Response</span></span>
<span data-ttu-id="6182e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6182e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



