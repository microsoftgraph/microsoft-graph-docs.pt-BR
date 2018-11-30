---
title: Atualizar iosVppApp
description: Atualiza as propriedades de um objeto iosVppApp.
ms.openlocfilehash: 8da21723bc8b10cb7bdfe1a2a6664f57f0bff7a9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003750"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="48626-103">Atualizar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="48626-103">Update iosVppApp</span></span>

> <span data-ttu-id="48626-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="48626-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48626-105">Atualiza as propriedades de um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="48626-105">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48626-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48626-106">Prerequisites</span></span>
<span data-ttu-id="48626-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48626-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48626-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48626-109">Permission type</span></span>|<span data-ttu-id="48626-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48626-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48626-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48626-111">Delegated (work or school account)</span></span>|<span data-ttu-id="48626-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48626-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48626-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48626-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48626-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48626-114">Not supported.</span></span>|
|<span data-ttu-id="48626-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48626-115">Application</span></span>|<span data-ttu-id="48626-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48626-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48626-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48626-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="48626-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48626-118">Request headers</span></span>
|<span data-ttu-id="48626-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48626-119">Header</span></span>|<span data-ttu-id="48626-120">Valor</span><span class="sxs-lookup"><span data-stu-id="48626-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48626-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="48626-121">Authorization</span></span>|<span data-ttu-id="48626-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48626-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48626-123">Accept</span><span class="sxs-lookup"><span data-stu-id="48626-123">Accept</span></span>|<span data-ttu-id="48626-124">application/json</span><span class="sxs-lookup"><span data-stu-id="48626-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48626-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48626-125">Request body</span></span>
<span data-ttu-id="48626-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="48626-126">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="48626-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="48626-127">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="48626-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48626-128">Property</span></span>|<span data-ttu-id="48626-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="48626-129">Type</span></span>|<span data-ttu-id="48626-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="48626-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48626-131">id</span><span class="sxs-lookup"><span data-stu-id="48626-131">id</span></span>|<span data-ttu-id="48626-132">String</span><span class="sxs-lookup"><span data-stu-id="48626-132">String</span></span>|<span data-ttu-id="48626-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="48626-133">Key of the entity.</span></span> <span data-ttu-id="48626-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-135">displayName</span><span class="sxs-lookup"><span data-stu-id="48626-135">displayName</span></span>|<span data-ttu-id="48626-136">String</span><span class="sxs-lookup"><span data-stu-id="48626-136">String</span></span>|<span data-ttu-id="48626-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="48626-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="48626-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-139">description</span><span class="sxs-lookup"><span data-stu-id="48626-139">description</span></span>|<span data-ttu-id="48626-140">String</span><span class="sxs-lookup"><span data-stu-id="48626-140">String</span></span>|<span data-ttu-id="48626-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48626-141">The description of the app.</span></span> <span data-ttu-id="48626-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-143">publisher</span><span class="sxs-lookup"><span data-stu-id="48626-143">publisher</span></span>|<span data-ttu-id="48626-144">String</span><span class="sxs-lookup"><span data-stu-id="48626-144">String</span></span>|<span data-ttu-id="48626-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48626-145">The publisher of the app.</span></span> <span data-ttu-id="48626-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="48626-147">largeIcon</span></span>|[<span data-ttu-id="48626-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="48626-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="48626-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="48626-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="48626-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48626-151">createdDateTime</span></span>|<span data-ttu-id="48626-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48626-152">DateTimeOffset</span></span>|<span data-ttu-id="48626-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48626-153">The date and time the app was created.</span></span> <span data-ttu-id="48626-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48626-155">lastModifiedDateTime</span></span>|<span data-ttu-id="48626-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48626-156">DateTimeOffset</span></span>|<span data-ttu-id="48626-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="48626-157">The date and time the app was last modified.</span></span> <span data-ttu-id="48626-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="48626-159">isFeatured</span></span>|<span data-ttu-id="48626-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="48626-160">Boolean</span></span>|<span data-ttu-id="48626-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="48626-162">privacyInformationUrl</span></span>|<span data-ttu-id="48626-163">String</span><span class="sxs-lookup"><span data-stu-id="48626-163">String</span></span>|<span data-ttu-id="48626-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="48626-164">The privacy statement Url.</span></span> <span data-ttu-id="48626-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="48626-166">informationUrl</span></span>|<span data-ttu-id="48626-167">String</span><span class="sxs-lookup"><span data-stu-id="48626-167">String</span></span>|<span data-ttu-id="48626-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="48626-168">The more information Url.</span></span> <span data-ttu-id="48626-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-170">owner</span><span class="sxs-lookup"><span data-stu-id="48626-170">owner</span></span>|<span data-ttu-id="48626-171">String</span><span class="sxs-lookup"><span data-stu-id="48626-171">String</span></span>|<span data-ttu-id="48626-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="48626-172">The owner of the app.</span></span> <span data-ttu-id="48626-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-174">developer</span><span class="sxs-lookup"><span data-stu-id="48626-174">developer</span></span>|<span data-ttu-id="48626-175">String</span><span class="sxs-lookup"><span data-stu-id="48626-175">String</span></span>|<span data-ttu-id="48626-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48626-176">The developer of the app.</span></span> <span data-ttu-id="48626-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-178">Observações</span><span class="sxs-lookup"><span data-stu-id="48626-178">notes</span></span>|<span data-ttu-id="48626-179">String</span><span class="sxs-lookup"><span data-stu-id="48626-179">String</span></span>|<span data-ttu-id="48626-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48626-180">Notes for the app.</span></span> <span data-ttu-id="48626-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48626-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48626-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="48626-182">publishingState</span></span>|[<span data-ttu-id="48626-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="48626-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="48626-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48626-184">The publishing state for the app.</span></span> <span data-ttu-id="48626-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="48626-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="48626-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48626-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="48626-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="48626-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="48626-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="48626-188">usedLicenseCount</span></span>|<span data-ttu-id="48626-189">Int32</span><span class="sxs-lookup"><span data-stu-id="48626-189">Int32</span></span>|<span data-ttu-id="48626-190">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="48626-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="48626-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="48626-191">totalLicenseCount</span></span>|<span data-ttu-id="48626-192">Int32</span><span class="sxs-lookup"><span data-stu-id="48626-192">Int32</span></span>|<span data-ttu-id="48626-193">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="48626-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="48626-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="48626-194">releaseDateTime</span></span>|<span data-ttu-id="48626-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48626-195">DateTimeOffset</span></span>|<span data-ttu-id="48626-196">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="48626-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="48626-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="48626-197">appStoreUrl</span></span>|<span data-ttu-id="48626-198">String</span><span class="sxs-lookup"><span data-stu-id="48626-198">String</span></span>|<span data-ttu-id="48626-199">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="48626-199">The store URL.</span></span>|
|<span data-ttu-id="48626-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="48626-200">licensingType</span></span>|[<span data-ttu-id="48626-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="48626-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="48626-202">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="48626-202">The supported License Type.</span></span>|
|<span data-ttu-id="48626-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="48626-203">applicableDeviceType</span></span>|[<span data-ttu-id="48626-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="48626-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="48626-205">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="48626-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="48626-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="48626-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="48626-207">String</span><span class="sxs-lookup"><span data-stu-id="48626-207">String</span></span>|<span data-ttu-id="48626-208">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="48626-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="48626-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="48626-209">vppTokenAccountType</span></span>|[<span data-ttu-id="48626-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="48626-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="48626-211">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="48626-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="48626-212">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="48626-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="48626-213">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="48626-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="48626-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="48626-214">vppTokenAppleId</span></span>|<span data-ttu-id="48626-215">String</span><span class="sxs-lookup"><span data-stu-id="48626-215">String</span></span>|<span data-ttu-id="48626-216">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="48626-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="48626-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="48626-217">bundleId</span></span>|<span data-ttu-id="48626-218">String</span><span class="sxs-lookup"><span data-stu-id="48626-218">String</span></span>|<span data-ttu-id="48626-219">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="48626-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="48626-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="48626-220">Response</span></span>
<span data-ttu-id="48626-221">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48626-221">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48626-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48626-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="48626-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48626-223">Request</span></span>
<span data-ttu-id="48626-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48626-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48626-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="48626-225">Response</span></span>
<span data-ttu-id="48626-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48626-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



