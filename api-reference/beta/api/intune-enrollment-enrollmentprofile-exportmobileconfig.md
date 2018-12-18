---
title: função exportMobileConfig
description: Exporta a configuração móvel
author: tfitzmac
ms.openlocfilehash: d6f663a729e45433c6f56f08ba02bb642749f5f5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350667"
---
# <a name="exportmobileconfig-function"></a><span data-ttu-id="dccdb-103">função exportMobileConfig</span><span class="sxs-lookup"><span data-stu-id="dccdb-103">exportMobileConfig function</span></span>

> <span data-ttu-id="dccdb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dccdb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dccdb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dccdb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dccdb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dccdb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dccdb-107">Exporta a configuração móvel</span><span class="sxs-lookup"><span data-stu-id="dccdb-107">Exports the mobile configuration</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dccdb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dccdb-108">Prerequisites</span></span>
<span data-ttu-id="dccdb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dccdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dccdb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dccdb-111">Permission type</span></span>|<span data-ttu-id="dccdb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dccdb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dccdb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dccdb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dccdb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dccdb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dccdb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dccdb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dccdb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dccdb-116">Not supported.</span></span>|
|<span data-ttu-id="dccdb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dccdb-117">Application</span></span>|<span data-ttu-id="dccdb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dccdb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dccdb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dccdb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

## <a name="request-headers"></a><span data-ttu-id="dccdb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dccdb-120">Request headers</span></span>
|<span data-ttu-id="dccdb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dccdb-121">Header</span></span>|<span data-ttu-id="dccdb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dccdb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dccdb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dccdb-123">Authorization</span></span>|<span data-ttu-id="dccdb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dccdb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dccdb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dccdb-125">Accept</span></span>|<span data-ttu-id="dccdb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dccdb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dccdb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dccdb-127">Request body</span></span>
<span data-ttu-id="dccdb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dccdb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dccdb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dccdb-129">Response</span></span>
<span data-ttu-id="dccdb-130">Se tiver êxito, esta função retornará um código de resposta `200 OK` e uma Cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dccdb-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dccdb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dccdb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dccdb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dccdb-132">Request</span></span>
<span data-ttu-id="dccdb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dccdb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

### <a name="response"></a><span data-ttu-id="dccdb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dccdb-134">Response</span></span>
<span data-ttu-id="dccdb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dccdb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Export Mobile Config value"
}
```





