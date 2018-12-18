---
title: Listar deviceEnrollmentConfigurations
description: Listar propriedades e relações de objetos de deviceEnrollmentConfiguration.
author: tfitzmac
ms.openlocfilehash: da1be6eb416e50654716fcd61a26443908ebc450
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351832"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="96874-103">Listar deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="96874-103">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="96874-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="96874-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96874-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="96874-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96874-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="96874-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96874-107">Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96874-107">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96874-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96874-108">Prerequisites</span></span>
<span data-ttu-id="96874-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96874-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96874-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96874-111">Permission type</span></span>|<span data-ttu-id="96874-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96874-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96874-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96874-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96874-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="96874-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="96874-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96874-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96874-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96874-116">Not supported.</span></span>|
|<span data-ttu-id="96874-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96874-117">Application</span></span>|<span data-ttu-id="96874-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96874-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96874-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96874-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="96874-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96874-120">Request headers</span></span>
|<span data-ttu-id="96874-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96874-121">Header</span></span>|<span data-ttu-id="96874-122">Valor</span><span class="sxs-lookup"><span data-stu-id="96874-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96874-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96874-123">Authorization</span></span>|<span data-ttu-id="96874-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96874-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96874-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96874-125">Accept</span></span>|<span data-ttu-id="96874-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96874-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96874-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96874-127">Request body</span></span>
<span data-ttu-id="96874-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96874-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96874-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="96874-129">Response</span></span>
<span data-ttu-id="96874-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96874-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96874-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96874-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="96874-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96874-132">Request</span></span>
<span data-ttu-id="96874-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96874-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="96874-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="96874-134">Response</span></span>
<span data-ttu-id="96874-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96874-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```





