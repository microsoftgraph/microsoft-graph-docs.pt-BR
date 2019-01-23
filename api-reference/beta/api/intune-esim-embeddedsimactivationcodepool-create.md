---
title: Criar embeddedSIMActivationCodePool
description: Crie um novo objeto de embeddedSIMActivationCodePool.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3b2d84230049c7b1f96756ac104557c5d8648c6a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394023"
---
# <a name="create-embeddedsimactivationcodepool"></a><span data-ttu-id="3115c-103">Criar embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="3115c-103">Create embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="3115c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="3115c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3115c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3115c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3115c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="3115c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3115c-107">Crie um novo objeto de [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="3115c-107">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3115c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3115c-108">Prerequisites</span></span>
<span data-ttu-id="3115c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3115c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3115c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3115c-111">Permission type</span></span>|<span data-ttu-id="3115c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3115c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3115c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3115c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3115c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3115c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3115c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3115c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3115c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3115c-116">Not supported.</span></span>|
|<span data-ttu-id="3115c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3115c-117">Application</span></span>|<span data-ttu-id="3115c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3115c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3115c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3115c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="3115c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3115c-120">Request headers</span></span>
|<span data-ttu-id="3115c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3115c-121">Header</span></span>|<span data-ttu-id="3115c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3115c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3115c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3115c-123">Authorization</span></span>|<span data-ttu-id="3115c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3115c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3115c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3115c-125">Accept</span></span>|<span data-ttu-id="3115c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3115c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3115c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3115c-127">Request body</span></span>
<span data-ttu-id="3115c-128">No corpo da solicitação, fornece uma representação JSON para o objeto embeddedSIMActivationCodePool.</span><span class="sxs-lookup"><span data-stu-id="3115c-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePool object.</span></span>

<span data-ttu-id="3115c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o embeddedSIMActivationCodePool.</span><span class="sxs-lookup"><span data-stu-id="3115c-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePool.</span></span>

|<span data-ttu-id="3115c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3115c-130">Property</span></span>|<span data-ttu-id="3115c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3115c-131">Type</span></span>|<span data-ttu-id="3115c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3115c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3115c-133">id</span><span class="sxs-lookup"><span data-stu-id="3115c-133">id</span></span>|<span data-ttu-id="3115c-134">String</span><span class="sxs-lookup"><span data-stu-id="3115c-134">String</span></span>|<span data-ttu-id="3115c-135">Identificador exclusivo para o pool de código de ativação SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="3115c-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="3115c-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="3115c-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="3115c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3115c-137">displayName</span></span>|<span data-ttu-id="3115c-138">String</span><span class="sxs-lookup"><span data-stu-id="3115c-138">String</span></span>|<span data-ttu-id="3115c-139">O administrador definida pelo nome do pool de código de ativação SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="3115c-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="3115c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3115c-140">createdDateTime</span></span>|<span data-ttu-id="3115c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3115c-141">DateTimeOffset</span></span>|<span data-ttu-id="3115c-142">A hora em que o pool de código de ativação SIM incorporado foi criado.</span><span class="sxs-lookup"><span data-stu-id="3115c-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="3115c-143">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="3115c-143">Generated service side.</span></span>|
|<span data-ttu-id="3115c-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3115c-144">modifiedDateTime</span></span>|<span data-ttu-id="3115c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3115c-145">DateTimeOffset</span></span>|<span data-ttu-id="3115c-146">A hora em que o pool de código de ativação SIM incorporado foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3115c-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="3115c-147">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="3115c-147">Updated service side.</span></span>|
|<span data-ttu-id="3115c-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="3115c-148">activationCodes</span></span>|<span data-ttu-id="3115c-149">coleção [embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)</span><span class="sxs-lookup"><span data-stu-id="3115c-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="3115c-150">Os códigos de ativação que pertencem a esse pool.</span><span class="sxs-lookup"><span data-stu-id="3115c-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="3115c-151">Esta propriedade de navegação é usada para postar códigos de ativação para Intune, mas não pode ser usada para ler códigos de ativação do Intune.</span><span class="sxs-lookup"><span data-stu-id="3115c-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="3115c-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="3115c-152">activationCodeCount</span></span>|<span data-ttu-id="3115c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3115c-153">Int32</span></span>|<span data-ttu-id="3115c-154">A contagem total dos códigos de ativação que pertencem a esse pool.</span><span class="sxs-lookup"><span data-stu-id="3115c-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="3115c-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="3115c-155">Response</span></span>
<span data-ttu-id="3115c-156">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3115c-156">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3115c-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3115c-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="3115c-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3115c-158">Request</span></span>
<span data-ttu-id="3115c-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3115c-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
Content-type: application/json
Content-length: 460

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### <a name="response"></a><span data-ttu-id="3115c-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="3115c-160">Response</span></span>
<span data-ttu-id="3115c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3115c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "ec308741-8741-ec30-4187-30ec418730ec",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```




