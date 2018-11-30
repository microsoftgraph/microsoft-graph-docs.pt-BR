---
title: Ação setMobileDeviceManagementAuthority
description: Define uma autoridade de gerenciamento de dispositivo móvel
ms.openlocfilehash: 31a0a23362a9d5c19b3022cff1d1567f591655d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033102"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="5c6dc-103">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="5c6dc-103">setMobileDeviceManagementAuthority action</span></span>

> <span data-ttu-id="5c6dc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5c6dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c6dc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5c6dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c6dc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5c6dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c6dc-107">Define uma autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="5c6dc-107">Set mobile device management authority</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c6dc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c6dc-108">Prerequisites</span></span>
<span data-ttu-id="5c6dc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c6dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c6dc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c6dc-111">Permission type</span></span>|<span data-ttu-id="5c6dc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c6dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c6dc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c6dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c6dc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c6dc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5c6dc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c6dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c6dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c6dc-116">Not supported.</span></span>|
|<span data-ttu-id="5c6dc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c6dc-117">Application</span></span>|<span data-ttu-id="5c6dc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c6dc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c6dc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c6dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="5c6dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c6dc-120">Request headers</span></span>
|<span data-ttu-id="5c6dc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c6dc-121">Header</span></span>|<span data-ttu-id="5c6dc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5c6dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c6dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c6dc-123">Authorization</span></span>|<span data-ttu-id="5c6dc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c6dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c6dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5c6dc-125">Accept</span></span>|<span data-ttu-id="5c6dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c6dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c6dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c6dc-127">Request body</span></span>
<span data-ttu-id="5c6dc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c6dc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c6dc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c6dc-129">Response</span></span>
<span data-ttu-id="5c6dc-130">Se tiver êxito, esta ação retorna o código de resposta `200 OK` e a Int32 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c6dc-130">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c6dc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c6dc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c6dc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c6dc-132">Request</span></span>
<span data-ttu-id="5c6dc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c6dc-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="5c6dc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c6dc-134">Response</span></span>
<span data-ttu-id="5c6dc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c6dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```





