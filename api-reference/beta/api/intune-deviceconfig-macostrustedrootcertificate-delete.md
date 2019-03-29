---
title: Excluir macOSTrustedRootCertificate
description: Exclui macOSTrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c84b5a97a9c84a0b4107e17bc8687c5b3602603e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970398"
---
# <a name="delete-macostrustedrootcertificate"></a><span data-ttu-id="7c118-103">Excluir macOSTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7c118-103">Delete macOSTrustedRootCertificate</span></span>

> <span data-ttu-id="7c118-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c118-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c118-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c118-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c118-106">Exclui [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="7c118-106">Deletes a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c118-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c118-107">Prerequisites</span></span>
<span data-ttu-id="7c118-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c118-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c118-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c118-110">Permission type</span></span>|<span data-ttu-id="7c118-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c118-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c118-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c118-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c118-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c118-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c118-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c118-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c118-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c118-115">Not supported.</span></span>|
|<span data-ttu-id="7c118-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c118-116">Application</span></span>|<span data-ttu-id="7c118-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c118-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c118-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c118-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="7c118-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c118-119">Request headers</span></span>
|<span data-ttu-id="7c118-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c118-120">Header</span></span>|<span data-ttu-id="7c118-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7c118-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c118-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c118-122">Authorization</span></span>|<span data-ttu-id="7c118-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c118-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c118-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c118-124">Accept</span></span>|<span data-ttu-id="7c118-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c118-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c118-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c118-126">Request body</span></span>
<span data-ttu-id="7c118-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c118-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c118-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c118-128">Response</span></span>
<span data-ttu-id="7c118-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7c118-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7c118-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c118-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c118-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c118-131">Request</span></span>
<span data-ttu-id="7c118-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c118-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
```

### <a name="response"></a><span data-ttu-id="7c118-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c118-133">Response</span></span>
<span data-ttu-id="7c118-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c118-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




