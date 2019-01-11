---
title: Ação setMobileDeviceManagementAuthority
description: Define uma autoridade de gerenciamento de dispositivo móvel
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8b488b500ac203dfed0582eadc738c15ecf41950
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889793"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="a69ee-103">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="a69ee-103">setMobileDeviceManagementAuthority action</span></span>

> <span data-ttu-id="a69ee-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a69ee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a69ee-105">Define uma autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="a69ee-105">Set mobile device management authority</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a69ee-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a69ee-106">Prerequisites</span></span>
<span data-ttu-id="a69ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a69ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a69ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a69ee-109">Permission type</span></span>|<span data-ttu-id="a69ee-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a69ee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a69ee-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a69ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a69ee-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a69ee-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a69ee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a69ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a69ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a69ee-114">Not supported.</span></span>|
|<span data-ttu-id="a69ee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a69ee-115">Application</span></span>|<span data-ttu-id="a69ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a69ee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a69ee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a69ee-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="a69ee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a69ee-118">Request headers</span></span>
|<span data-ttu-id="a69ee-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a69ee-119">Header</span></span>|<span data-ttu-id="a69ee-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a69ee-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a69ee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a69ee-121">Authorization</span></span>|<span data-ttu-id="a69ee-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a69ee-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a69ee-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a69ee-123">Accept</span></span>|<span data-ttu-id="a69ee-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a69ee-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a69ee-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a69ee-125">Request body</span></span>
<span data-ttu-id="a69ee-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a69ee-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a69ee-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a69ee-127">Response</span></span>
<span data-ttu-id="a69ee-128">Se tiver êxito, esta ação retorna o código de resposta `200 OK` e a Int32 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a69ee-128">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a69ee-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a69ee-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a69ee-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a69ee-130">Request</span></span>
<span data-ttu-id="a69ee-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a69ee-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="a69ee-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a69ee-132">Response</span></span>
<span data-ttu-id="a69ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a69ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```



