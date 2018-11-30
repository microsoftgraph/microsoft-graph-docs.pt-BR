---
title: Lista windowsDomainJoinConfigurations
description: Lista as propriedades e os relacionamentos dos objetos windowsDomainJoinConfiguration.
ms.openlocfilehash: b4708533f0f8c52a4ebc6f962db45f4f04f95d73
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036673"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="9853a-103">Lista windowsDomainJoinConfigurations</span><span class="sxs-lookup"><span data-stu-id="9853a-103">List windowsDomainJoinConfigurations</span></span>

> <span data-ttu-id="9853a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9853a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9853a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9853a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9853a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9853a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9853a-107">Lista as propriedades e os relacionamentos dos objetos [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9853a-107">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9853a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9853a-108">Prerequisites</span></span>
<span data-ttu-id="9853a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9853a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9853a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9853a-111">Permission type</span></span>|<span data-ttu-id="9853a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9853a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9853a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9853a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9853a-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="9853a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="9853a-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9853a-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9853a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9853a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9853a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9853a-117">Not supported.</span></span>|
|<span data-ttu-id="9853a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9853a-118">Application</span></span>|<span data-ttu-id="9853a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9853a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9853a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9853a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9853a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9853a-121">Request headers</span></span>
|<span data-ttu-id="9853a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9853a-122">Header</span></span>|<span data-ttu-id="9853a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9853a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9853a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9853a-124">Authorization</span></span>|<span data-ttu-id="9853a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9853a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9853a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9853a-126">Accept</span></span>|<span data-ttu-id="9853a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9853a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9853a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9853a-128">Request body</span></span>
<span data-ttu-id="9853a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9853a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9853a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9853a-130">Response</span></span>
<span data-ttu-id="9853a-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9853a-131">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9853a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9853a-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="9853a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9853a-133">Request</span></span>
<span data-ttu-id="9853a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9853a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9853a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9853a-135">Response</span></span>
<span data-ttu-id="9853a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9853a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



