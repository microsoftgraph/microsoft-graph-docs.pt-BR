---
title: ação setAndroidDeviceOwnerFullyManagedEnrollmentState
description: Define o AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled para o valor especificado.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 772a52f43a36eed4c7d910adcb44c3d614733546
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417937"
---
# <a name="setandroiddeviceownerfullymanagedenrollmentstate-action"></a><span data-ttu-id="ea19e-103">ação setAndroidDeviceOwnerFullyManagedEnrollmentState</span><span class="sxs-lookup"><span data-stu-id="ea19e-103">setAndroidDeviceOwnerFullyManagedEnrollmentState action</span></span>

<span data-ttu-id="ea19e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea19e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea19e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea19e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea19e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea19e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea19e-107">Define o AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled para o valor especificado.</span><span class="sxs-lookup"><span data-stu-id="ea19e-107">Sets the AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled to the given value.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea19e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ea19e-108">Prerequisites</span></span>
<span data-ttu-id="ea19e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea19e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea19e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea19e-111">Permission type</span></span>|<span data-ttu-id="ea19e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ea19e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea19e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea19e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea19e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea19e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea19e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea19e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea19e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea19e-116">Not supported.</span></span>|
|<span data-ttu-id="ea19e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea19e-117">Application</span></span>|<span data-ttu-id="ea19e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea19e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea19e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea19e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState
```

## <a name="request-headers"></a><span data-ttu-id="ea19e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea19e-120">Request headers</span></span>
|<span data-ttu-id="ea19e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea19e-121">Header</span></span>|<span data-ttu-id="ea19e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ea19e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea19e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea19e-123">Authorization</span></span>|<span data-ttu-id="ea19e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea19e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea19e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ea19e-125">Accept</span></span>|<span data-ttu-id="ea19e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea19e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea19e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea19e-127">Request body</span></span>
<span data-ttu-id="ea19e-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ea19e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ea19e-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ea19e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ea19e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea19e-130">Property</span></span>|<span data-ttu-id="ea19e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea19e-131">Type</span></span>|<span data-ttu-id="ea19e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea19e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea19e-133">enabled</span><span class="sxs-lookup"><span data-stu-id="ea19e-133">enabled</span></span>|<span data-ttu-id="ea19e-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea19e-134">Boolean</span></span>|<span data-ttu-id="ea19e-135">O valor para o qual definir AndroidDeviceOwnerFullyManagedEnrollmentEnabled.</span><span class="sxs-lookup"><span data-stu-id="ea19e-135">The value to set AndroidDeviceOwnerFullyManagedEnrollmentEnabled to.</span></span>|



## <a name="response"></a><span data-ttu-id="ea19e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea19e-136">Response</span></span>
<span data-ttu-id="ea19e-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ea19e-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ea19e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea19e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea19e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea19e-139">Request</span></span>
<span data-ttu-id="ea19e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea19e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState

Content-type: application/json
Content-length: 23

{
  "enabled": true
}
```

### <a name="response"></a><span data-ttu-id="ea19e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea19e-141">Response</span></span>
<span data-ttu-id="ea19e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea19e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



