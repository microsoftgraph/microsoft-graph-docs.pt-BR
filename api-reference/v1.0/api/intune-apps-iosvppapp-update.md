---
title: Atualizar iosVppApp
description: Atualiza as propriedades de um objeto iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 777b92cb56c61889f463b28c14e54c8300491242
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27992074"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="f8036-103">Atualizar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="f8036-103">Update iosVppApp</span></span>

> <span data-ttu-id="f8036-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f8036-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8036-105">Atualiza as propriedades de um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="f8036-105">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8036-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8036-106">Prerequisites</span></span>
<span data-ttu-id="f8036-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8036-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8036-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8036-109">Permission type</span></span>|<span data-ttu-id="f8036-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8036-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8036-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8036-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f8036-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8036-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f8036-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8036-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8036-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8036-114">Not supported.</span></span>|
|<span data-ttu-id="f8036-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8036-115">Application</span></span>|<span data-ttu-id="f8036-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8036-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8036-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8036-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f8036-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8036-118">Request headers</span></span>
|<span data-ttu-id="f8036-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8036-119">Header</span></span>|<span data-ttu-id="f8036-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f8036-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8036-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8036-121">Authorization</span></span>|<span data-ttu-id="f8036-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8036-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8036-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8036-123">Accept</span></span>|<span data-ttu-id="f8036-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f8036-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8036-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8036-125">Request body</span></span>
<span data-ttu-id="f8036-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="f8036-126">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="f8036-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="f8036-127">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="f8036-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8036-128">Property</span></span>|<span data-ttu-id="f8036-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8036-129">Type</span></span>|<span data-ttu-id="f8036-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8036-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8036-131">id</span><span class="sxs-lookup"><span data-stu-id="f8036-131">id</span></span>|<span data-ttu-id="f8036-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-132">String</span></span>|<span data-ttu-id="f8036-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f8036-133">Key of the entity.</span></span> <span data-ttu-id="f8036-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f8036-135">displayName</span></span>|<span data-ttu-id="f8036-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-136">String</span></span>|<span data-ttu-id="f8036-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f8036-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f8036-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-139">description</span><span class="sxs-lookup"><span data-stu-id="f8036-139">description</span></span>|<span data-ttu-id="f8036-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-140">String</span></span>|<span data-ttu-id="f8036-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8036-141">The description of the app.</span></span> <span data-ttu-id="f8036-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-143">publisher</span><span class="sxs-lookup"><span data-stu-id="f8036-143">publisher</span></span>|<span data-ttu-id="f8036-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-144">String</span></span>|<span data-ttu-id="f8036-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8036-145">The publisher of the app.</span></span> <span data-ttu-id="f8036-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f8036-147">largeIcon</span></span>|[<span data-ttu-id="f8036-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f8036-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f8036-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f8036-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f8036-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8036-151">createdDateTime</span></span>|<span data-ttu-id="f8036-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8036-152">DateTimeOffset</span></span>|<span data-ttu-id="f8036-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8036-153">The date and time the app was created.</span></span> <span data-ttu-id="f8036-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8036-155">lastModifiedDateTime</span></span>|<span data-ttu-id="f8036-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8036-156">DateTimeOffset</span></span>|<span data-ttu-id="f8036-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f8036-157">The date and time the app was last modified.</span></span> <span data-ttu-id="f8036-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f8036-159">isFeatured</span></span>|<span data-ttu-id="f8036-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="f8036-160">Boolean</span></span>|<span data-ttu-id="f8036-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f8036-162">privacyInformationUrl</span></span>|<span data-ttu-id="f8036-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-163">String</span></span>|<span data-ttu-id="f8036-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f8036-164">The privacy statement Url.</span></span> <span data-ttu-id="f8036-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f8036-166">informationUrl</span></span>|<span data-ttu-id="f8036-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-167">String</span></span>|<span data-ttu-id="f8036-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f8036-168">The more information Url.</span></span> <span data-ttu-id="f8036-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-170">owner</span><span class="sxs-lookup"><span data-stu-id="f8036-170">owner</span></span>|<span data-ttu-id="f8036-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-171">String</span></span>|<span data-ttu-id="f8036-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f8036-172">The owner of the app.</span></span> <span data-ttu-id="f8036-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-174">developer</span><span class="sxs-lookup"><span data-stu-id="f8036-174">developer</span></span>|<span data-ttu-id="f8036-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-175">String</span></span>|<span data-ttu-id="f8036-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8036-176">The developer of the app.</span></span> <span data-ttu-id="f8036-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-178">Observações</span><span class="sxs-lookup"><span data-stu-id="f8036-178">notes</span></span>|<span data-ttu-id="f8036-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-179">String</span></span>|<span data-ttu-id="f8036-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8036-180">Notes for the app.</span></span> <span data-ttu-id="f8036-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f8036-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8036-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="f8036-182">publishingState</span></span>|[<span data-ttu-id="f8036-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f8036-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f8036-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8036-184">The publishing state for the app.</span></span> <span data-ttu-id="f8036-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f8036-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f8036-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f8036-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f8036-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f8036-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f8036-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f8036-188">usedLicenseCount</span></span>|<span data-ttu-id="f8036-189">Int32</span><span class="sxs-lookup"><span data-stu-id="f8036-189">Int32</span></span>|<span data-ttu-id="f8036-190">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="f8036-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="f8036-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f8036-191">totalLicenseCount</span></span>|<span data-ttu-id="f8036-192">Int32</span><span class="sxs-lookup"><span data-stu-id="f8036-192">Int32</span></span>|<span data-ttu-id="f8036-193">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="f8036-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="f8036-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="f8036-194">releaseDateTime</span></span>|<span data-ttu-id="f8036-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8036-195">DateTimeOffset</span></span>|<span data-ttu-id="f8036-196">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="f8036-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="f8036-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f8036-197">appStoreUrl</span></span>|<span data-ttu-id="f8036-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-198">String</span></span>|<span data-ttu-id="f8036-199">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="f8036-199">The store URL.</span></span>|
|<span data-ttu-id="f8036-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="f8036-200">licensingType</span></span>|[<span data-ttu-id="f8036-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="f8036-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="f8036-202">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="f8036-202">The supported License Type.</span></span>|
|<span data-ttu-id="f8036-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f8036-203">applicableDeviceType</span></span>|[<span data-ttu-id="f8036-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f8036-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f8036-205">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="f8036-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="f8036-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="f8036-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="f8036-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-207">String</span></span>|<span data-ttu-id="f8036-208">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="f8036-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="f8036-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f8036-209">vppTokenAccountType</span></span>|[<span data-ttu-id="f8036-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f8036-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="f8036-211">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="f8036-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="f8036-212">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="f8036-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="f8036-213">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="f8036-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="f8036-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="f8036-214">vppTokenAppleId</span></span>|<span data-ttu-id="f8036-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-215">String</span></span>|<span data-ttu-id="f8036-216">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="f8036-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f8036-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="f8036-217">bundleId</span></span>|<span data-ttu-id="f8036-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8036-218">String</span></span>|<span data-ttu-id="f8036-219">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f8036-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="f8036-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8036-220">Response</span></span>
<span data-ttu-id="f8036-221">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8036-221">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8036-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8036-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8036-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8036-223">Request</span></span>
<span data-ttu-id="f8036-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8036-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1222

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="f8036-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8036-225">Response</span></span>
<span data-ttu-id="f8036-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8036-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```



