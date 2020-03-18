---
title: função getEncryptionPublicKey
description: Obter uma chave pública para usar para criptografar o token do programa de registro de dispositivo Apple
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 495b24472bd36672710de8df765da78af61d7a0f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813250"
---
# <a name="getencryptionpublickey-function"></a><span data-ttu-id="e7078-103">função getEncryptionPublicKey</span><span class="sxs-lookup"><span data-stu-id="e7078-103">getEncryptionPublicKey function</span></span>

> <span data-ttu-id="e7078-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7078-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7078-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7078-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7078-106">Obter uma chave pública para usar para criptografar o token do programa de registro de dispositivo Apple</span><span class="sxs-lookup"><span data-stu-id="e7078-106">Get a public key to use to encrypt the Apple device enrollment program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7078-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7078-107">Prerequisites</span></span>
<span data-ttu-id="e7078-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7078-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7078-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7078-110">Permission type</span></span>|<span data-ttu-id="e7078-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7078-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7078-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7078-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7078-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7078-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e7078-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7078-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7078-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7078-115">Not supported.</span></span>|
|<span data-ttu-id="e7078-116">Application</span><span class="sxs-lookup"><span data-stu-id="e7078-116">Application</span></span>|<span data-ttu-id="e7078-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7078-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7078-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7078-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

## <a name="request-headers"></a><span data-ttu-id="e7078-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7078-119">Request headers</span></span>
|<span data-ttu-id="e7078-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7078-120">Header</span></span>|<span data-ttu-id="e7078-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e7078-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7078-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7078-122">Authorization</span></span>|<span data-ttu-id="e7078-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7078-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7078-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7078-124">Accept</span></span>|<span data-ttu-id="e7078-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7078-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7078-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7078-126">Request body</span></span>
<span data-ttu-id="e7078-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7078-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7078-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7078-128">Response</span></span>
<span data-ttu-id="e7078-129">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7078-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7078-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7078-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7078-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7078-131">Request</span></span>
<span data-ttu-id="e7078-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7078-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

### <a name="response"></a><span data-ttu-id="e7078-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7078-133">Response</span></span>
<span data-ttu-id="e7078-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7078-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 50

{
  "value": "Get Encryption Public Key value"
}
```




