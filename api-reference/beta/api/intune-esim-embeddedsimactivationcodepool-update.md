---
title: Atualizar embeddedSIMActivationCodePool
description: Atualize as propriedades de um objeto embeddedSIMActivationCodePool.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1758d832dfbc9fdbc2db1a65259f30c3662b5964
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942931"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="e416d-103">Atualizar embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="e416d-103">Update embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="e416d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e416d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e416d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e416d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e416d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e416d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e416d-107">Atualize as propriedades de um objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="e416d-107">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e416d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e416d-108">Prerequisites</span></span>
<span data-ttu-id="e416d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e416d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e416d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e416d-111">Permission type</span></span>|<span data-ttu-id="e416d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e416d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e416d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e416d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e416d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e416d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e416d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e416d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e416d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e416d-116">Not supported.</span></span>|
|<span data-ttu-id="e416d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e416d-117">Application</span></span>|<span data-ttu-id="e416d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e416d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e416d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e416d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="e416d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e416d-120">Request headers</span></span>
|<span data-ttu-id="e416d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e416d-121">Header</span></span>|<span data-ttu-id="e416d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e416d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e416d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e416d-123">Authorization</span></span>|<span data-ttu-id="e416d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e416d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e416d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e416d-125">Accept</span></span>|<span data-ttu-id="e416d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e416d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e416d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e416d-127">Request body</span></span>
<span data-ttu-id="e416d-128">No corpo da solicitação, fornece uma representação JSON para o objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="e416d-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="e416d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span><span class="sxs-lookup"><span data-stu-id="e416d-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="e416d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e416d-130">Property</span></span>|<span data-ttu-id="e416d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e416d-131">Type</span></span>|<span data-ttu-id="e416d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e416d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e416d-133">id</span><span class="sxs-lookup"><span data-stu-id="e416d-133">id</span></span>|<span data-ttu-id="e416d-134">String</span><span class="sxs-lookup"><span data-stu-id="e416d-134">String</span></span>|<span data-ttu-id="e416d-135">Identificador exclusivo para o pool de código de ativação SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="e416d-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="e416d-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="e416d-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="e416d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e416d-137">displayName</span></span>|<span data-ttu-id="e416d-138">String</span><span class="sxs-lookup"><span data-stu-id="e416d-138">String</span></span>|<span data-ttu-id="e416d-139">O administrador definida pelo nome do pool de código de ativação SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="e416d-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="e416d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e416d-140">createdDateTime</span></span>|<span data-ttu-id="e416d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e416d-141">DateTimeOffset</span></span>|<span data-ttu-id="e416d-142">A hora em que o pool de código de ativação SIM incorporado foi criado.</span><span class="sxs-lookup"><span data-stu-id="e416d-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="e416d-143">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="e416d-143">Generated service side.</span></span>|
|<span data-ttu-id="e416d-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e416d-144">modifiedDateTime</span></span>|<span data-ttu-id="e416d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e416d-145">DateTimeOffset</span></span>|<span data-ttu-id="e416d-146">A hora em que o pool de código de ativação SIM incorporado foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e416d-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="e416d-147">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="e416d-147">Updated service side.</span></span>|
|<span data-ttu-id="e416d-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="e416d-148">activationCodes</span></span>|<span data-ttu-id="e416d-149">coleção [embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)</span><span class="sxs-lookup"><span data-stu-id="e416d-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="e416d-150">Os códigos de ativação que pertencem a esse pool.</span><span class="sxs-lookup"><span data-stu-id="e416d-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="e416d-151">Esta propriedade de navegação é usada para postar códigos de ativação para Intune, mas não pode ser usada para ler códigos de ativação do Intune.</span><span class="sxs-lookup"><span data-stu-id="e416d-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="e416d-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="e416d-152">activationCodeCount</span></span>|<span data-ttu-id="e416d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e416d-153">Int32</span></span>|<span data-ttu-id="e416d-154">A contagem total dos códigos de ativação que pertencem a esse pool.</span><span class="sxs-lookup"><span data-stu-id="e416d-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="e416d-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e416d-155">Response</span></span>
<span data-ttu-id="e416d-156">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e416d-156">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e416d-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e416d-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="e416d-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e416d-158">Request</span></span>
<span data-ttu-id="e416d-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e416d-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
Content-type: application/json
Content-length: 392

{
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

### <a name="response"></a><span data-ttu-id="e416d-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e416d-160">Response</span></span>
<span data-ttu-id="e416d-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e416d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





