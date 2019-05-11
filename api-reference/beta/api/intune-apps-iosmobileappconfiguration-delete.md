---
title: Excluir iosMobileAppConfiguration
description: Exclui um iosMobileAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f29b60f420182f762c2a913e95a070f1d1600c8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33937012"
---
# <a name="delete-iosmobileappconfiguration"></a><span data-ttu-id="3c554-103">Excluir iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3c554-103">Delete iosMobileAppConfiguration</span></span>

> <span data-ttu-id="3c554-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c554-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c554-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c554-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c554-106">Exclui um [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c554-106">Deletes a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c554-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c554-107">Prerequisites</span></span>
<span data-ttu-id="3c554-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c554-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c554-110">Permission type</span></span>|<span data-ttu-id="3c554-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c554-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c554-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c554-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c554-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c554-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c554-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c554-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c554-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c554-115">Not supported.</span></span>|
|<span data-ttu-id="3c554-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c554-116">Application</span></span>|<span data-ttu-id="3c554-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c554-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c554-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c554-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3c554-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c554-119">Request headers</span></span>
|<span data-ttu-id="3c554-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c554-120">Header</span></span>|<span data-ttu-id="3c554-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3c554-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c554-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c554-122">Authorization</span></span>|<span data-ttu-id="3c554-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c554-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c554-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c554-124">Accept</span></span>|<span data-ttu-id="3c554-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c554-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c554-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c554-126">Request body</span></span>
<span data-ttu-id="3c554-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c554-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c554-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c554-128">Response</span></span>
<span data-ttu-id="3c554-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3c554-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3c554-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c554-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c554-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c554-131">Request</span></span>
<span data-ttu-id="3c554-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c554-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3c554-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c554-133">Response</span></span>
<span data-ttu-id="3c554-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c554-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




