---
title: Lista windowsDomainJoinConfigurations
description: Lista as propriedades e os relacionamentos dos objetos windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6aa69b7d880000923970a0ea5443633876a93ad8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925333"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="7e9ad-103">Lista windowsDomainJoinConfigurations</span><span class="sxs-lookup"><span data-stu-id="7e9ad-103">List windowsDomainJoinConfigurations</span></span>

> <span data-ttu-id="7e9ad-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7e9ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e9ad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7e9ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e9ad-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7e9ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e9ad-107">Lista as propriedades e os relacionamentos dos objetos [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7e9ad-107">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e9ad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7e9ad-108">Prerequisites</span></span>
<span data-ttu-id="7e9ad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e9ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e9ad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e9ad-111">Permission type</span></span>|<span data-ttu-id="7e9ad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7e9ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e9ad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e9ad-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7e9ad-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="7e9ad-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7e9ad-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e9ad-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7e9ad-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e9ad-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e9ad-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e9ad-117">Not supported.</span></span>|
|<span data-ttu-id="7e9ad-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e9ad-118">Application</span></span>|<span data-ttu-id="7e9ad-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e9ad-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e9ad-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e9ad-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7e9ad-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9ad-121">Request headers</span></span>
|<span data-ttu-id="7e9ad-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e9ad-122">Header</span></span>|<span data-ttu-id="7e9ad-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7e9ad-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e9ad-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e9ad-124">Authorization</span></span>|<span data-ttu-id="7e9ad-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e9ad-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e9ad-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7e9ad-126">Accept</span></span>|<span data-ttu-id="7e9ad-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7e9ad-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e9ad-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9ad-128">Request body</span></span>
<span data-ttu-id="7e9ad-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e9ad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e9ad-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e9ad-130">Response</span></span>
<span data-ttu-id="7e9ad-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e9ad-131">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e9ad-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e9ad-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e9ad-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9ad-133">Request</span></span>
<span data-ttu-id="7e9ad-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e9ad-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="7e9ad-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e9ad-135">Response</span></span>
<span data-ttu-id="7e9ad-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e9ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



