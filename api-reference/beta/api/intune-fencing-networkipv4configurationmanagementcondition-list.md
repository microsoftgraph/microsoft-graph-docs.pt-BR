---
title: Lista networkIPv4ConfigurationManagementConditions
description: Lista as propriedades e os relacionamentos dos objetos networkIPv4ConfigurationManagementCondition.
author: tfitzmac
ms.openlocfilehash: 6e1707fa85788fb5085f37654645b0863b5a8b46
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363610"
---
# <a name="list-networkipv4configurationmanagementconditions"></a><span data-ttu-id="7fb13-103">Lista networkIPv4ConfigurationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="7fb13-103">List networkIPv4ConfigurationManagementConditions</span></span>

> <span data-ttu-id="7fb13-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7fb13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fb13-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7fb13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fb13-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7fb13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fb13-107">Lista as propriedades e os relacionamentos dos objetos [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="7fb13-107">List properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7fb13-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7fb13-108">Prerequisites</span></span>
<span data-ttu-id="7fb13-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fb13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fb13-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fb13-111">Permission type</span></span>|<span data-ttu-id="7fb13-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7fb13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fb13-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fb13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7fb13-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fb13-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7fb13-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fb13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fb13-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fb13-116">Not supported.</span></span>|
|<span data-ttu-id="7fb13-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fb13-117">Application</span></span>|<span data-ttu-id="7fb13-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fb13-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fb13-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fb13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="7fb13-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb13-120">Request headers</span></span>
|<span data-ttu-id="7fb13-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fb13-121">Header</span></span>|<span data-ttu-id="7fb13-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7fb13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fb13-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fb13-123">Authorization</span></span>|<span data-ttu-id="7fb13-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fb13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fb13-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7fb13-125">Accept</span></span>|<span data-ttu-id="7fb13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7fb13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fb13-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb13-127">Request body</span></span>
<span data-ttu-id="7fb13-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7fb13-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fb13-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fb13-129">Response</span></span>
<span data-ttu-id="7fb13-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fb13-130">If successful, this method returns a `200 OK` response code and a collection of [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fb13-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fb13-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7fb13-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb13-132">Request</span></span>
<span data-ttu-id="7fb13-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fb13-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="7fb13-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fb13-134">Response</span></span>
<span data-ttu-id="7fb13-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fb13-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
      "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ],
      "ipV4Prefix": "Ip V4Prefix value",
      "ipV4Gateway": "Ip V4Gateway value",
      "ipV4DHCPServer": "Ip V4DHCPServer value",
      "ipV4DNSServerList": [
        "Ip V4DNSServer List value"
      ],
      "dnsSuffixList": [
        "Dns Suffix List value"
      ]
    }
  ]
}
```





