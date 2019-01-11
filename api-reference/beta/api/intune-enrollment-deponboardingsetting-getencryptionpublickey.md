---
title: função getEncryptionPublicKey
description: Obtenha uma chave pública para usar para criptografar o programa de inscrição do dispositivo Apple token
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eb373b862dc39d9636e59bf32ba00b84b7bf5563
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807627"
---
# <a name="getencryptionpublickey-function"></a><span data-ttu-id="95c1d-103">função getEncryptionPublicKey</span><span class="sxs-lookup"><span data-stu-id="95c1d-103">getEncryptionPublicKey function</span></span>

> <span data-ttu-id="95c1d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="95c1d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95c1d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="95c1d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95c1d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="95c1d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95c1d-107">Obtenha uma chave pública para usar para criptografar o programa de inscrição do dispositivo Apple token</span><span class="sxs-lookup"><span data-stu-id="95c1d-107">Get a public key to use to encrypt the Apple device enrollment program token</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95c1d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95c1d-108">Prerequisites</span></span>
<span data-ttu-id="95c1d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95c1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95c1d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95c1d-111">Permission type</span></span>|<span data-ttu-id="95c1d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="95c1d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95c1d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95c1d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95c1d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="95c1d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="95c1d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95c1d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95c1d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95c1d-116">Not supported.</span></span>|
|<span data-ttu-id="95c1d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95c1d-117">Application</span></span>|<span data-ttu-id="95c1d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95c1d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95c1d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95c1d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

## <a name="request-headers"></a><span data-ttu-id="95c1d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95c1d-120">Request headers</span></span>
|<span data-ttu-id="95c1d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95c1d-121">Header</span></span>|<span data-ttu-id="95c1d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="95c1d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95c1d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95c1d-123">Authorization</span></span>|<span data-ttu-id="95c1d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95c1d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95c1d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="95c1d-125">Accept</span></span>|<span data-ttu-id="95c1d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95c1d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95c1d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95c1d-127">Request body</span></span>
<span data-ttu-id="95c1d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95c1d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95c1d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c1d-129">Response</span></span>
<span data-ttu-id="95c1d-130">Se tiver êxito, esta função retornará um código de resposta `200 OK` e uma Cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95c1d-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95c1d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95c1d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="95c1d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95c1d-132">Request</span></span>
<span data-ttu-id="95c1d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95c1d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

### <a name="response"></a><span data-ttu-id="95c1d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c1d-134">Response</span></span>
<span data-ttu-id="95c1d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95c1d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 50

{
  "value": "Get Encryption Public Key value"
}
```





