---
title: Excluir deviceEnrollmentPlatformRestrictionsConfiguration
description: Exclui deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c168790421feca623426b88988a87847a4d00ef8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582756"
---
# <a name="delete-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="86018-103">Excluir deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="86018-103">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="86018-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86018-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86018-105">Exclui [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86018-105">Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86018-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86018-106">Prerequisites</span></span>
<span data-ttu-id="86018-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86018-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86018-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86018-109">Permission type</span></span>|<span data-ttu-id="86018-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86018-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86018-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86018-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86018-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86018-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="86018-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86018-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86018-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86018-114">Not supported.</span></span>|
|<span data-ttu-id="86018-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86018-115">Application</span></span>|<span data-ttu-id="86018-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86018-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86018-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86018-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="86018-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86018-118">Request headers</span></span>
|<span data-ttu-id="86018-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86018-119">Header</span></span>|<span data-ttu-id="86018-120">Valor</span><span class="sxs-lookup"><span data-stu-id="86018-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86018-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="86018-121">Authorization</span></span>|<span data-ttu-id="86018-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86018-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86018-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86018-123">Accept</span></span>|<span data-ttu-id="86018-124">application/json</span><span class="sxs-lookup"><span data-stu-id="86018-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86018-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86018-125">Request body</span></span>
<span data-ttu-id="86018-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86018-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86018-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="86018-127">Response</span></span>
<span data-ttu-id="86018-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="86018-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="86018-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86018-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="86018-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86018-130">Request</span></span>
<span data-ttu-id="86018-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86018-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="86018-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="86018-132">Response</span></span>
<span data-ttu-id="86018-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86018-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



