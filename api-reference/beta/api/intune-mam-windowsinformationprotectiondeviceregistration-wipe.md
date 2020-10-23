---
title: Ação wipe
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 19682cde1010fbf6097d9eb66aa31c4300c712f6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722533"
---
# <a name="wipe-action"></a><span data-ttu-id="2c021-103">ação wipe</span><span class="sxs-lookup"><span data-stu-id="2c021-103">wipe action</span></span>

<span data-ttu-id="2c021-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c021-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c021-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c021-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c021-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c021-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c021-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2c021-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c021-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2c021-108">Prerequisites</span></span>
<span data-ttu-id="2c021-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c021-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c021-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c021-111">Permission type</span></span>|<span data-ttu-id="2c021-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2c021-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c021-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c021-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c021-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c021-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2c021-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c021-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c021-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c021-116">Not supported.</span></span>|
|<span data-ttu-id="2c021-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c021-117">Application</span></span>|<span data-ttu-id="2c021-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c021-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c021-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c021-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="2c021-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c021-120">Request headers</span></span>
|<span data-ttu-id="2c021-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c021-121">Header</span></span>|<span data-ttu-id="2c021-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2c021-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c021-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c021-123">Authorization</span></span>|<span data-ttu-id="2c021-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c021-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c021-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2c021-125">Accept</span></span>|<span data-ttu-id="2c021-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c021-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c021-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c021-127">Request body</span></span>
<span data-ttu-id="2c021-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c021-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c021-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c021-129">Response</span></span>
<span data-ttu-id="2c021-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2c021-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2c021-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c021-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c021-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c021-132">Request</span></span>
<span data-ttu-id="2c021-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c021-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}/wipe
```

### <a name="response"></a><span data-ttu-id="2c021-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c021-134">Response</span></span>
<span data-ttu-id="2c021-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c021-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





