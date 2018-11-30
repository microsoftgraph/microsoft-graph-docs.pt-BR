---
title: Lista androidForWorkGmailEasConfigurations
description: Lista as propriedades e os relacionamentos dos objetos androidForWorkGmailEasConfiguration.
ms.openlocfilehash: a8d575ee5dcad9b1e6eeec8027364e28d25c7134
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033263"
---
# <a name="list-androidforworkgmaileasconfigurations"></a><span data-ttu-id="d7880-103">Lista androidForWorkGmailEasConfigurations</span><span class="sxs-lookup"><span data-stu-id="d7880-103">List androidForWorkGmailEasConfigurations</span></span>

> <span data-ttu-id="d7880-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d7880-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7880-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d7880-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7880-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d7880-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7880-107">Lista as propriedades e os relacionamentos dos objetos [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d7880-107">List properties and relationships of the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7880-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7880-108">Prerequisites</span></span>
<span data-ttu-id="d7880-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7880-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7880-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7880-111">Permission type</span></span>|<span data-ttu-id="d7880-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7880-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7880-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7880-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7880-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7880-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d7880-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7880-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7880-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7880-116">Not supported.</span></span>|
|<span data-ttu-id="d7880-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7880-117">Application</span></span>|<span data-ttu-id="d7880-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7880-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7880-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7880-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d7880-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7880-120">Request headers</span></span>
|<span data-ttu-id="d7880-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7880-121">Header</span></span>|<span data-ttu-id="d7880-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d7880-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7880-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7880-123">Authorization</span></span>|<span data-ttu-id="d7880-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7880-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7880-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7880-125">Accept</span></span>|<span data-ttu-id="d7880-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7880-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7880-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7880-127">Request body</span></span>
<span data-ttu-id="d7880-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7880-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7880-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7880-129">Response</span></span>
<span data-ttu-id="d7880-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7880-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7880-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7880-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7880-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7880-132">Request</span></span>
<span data-ttu-id="d7880-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7880-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d7880-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7880-134">Response</span></span>
<span data-ttu-id="d7880-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7880-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 764

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
      "id": "2bafc891-c891-2baf-91c8-af2b91c8af2b",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "authenticationMethod": "certificate",
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "hostName": "Host Name value",
      "requireSsl": true,
      "usernameSource": "userPrincipalName"
    }
  ]
}
```





