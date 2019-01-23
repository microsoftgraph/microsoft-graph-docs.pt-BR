---
title: Criar androidForWorkApp
description: Crie um novo objeto de androidForWorkApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dad21f184ff5cfdd31ef4ed8114169850b2239c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401835"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="3f603-103">Criar androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="3f603-103">Create androidForWorkApp</span></span>

> <span data-ttu-id="3f603-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="3f603-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3f603-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3f603-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f603-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="3f603-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f603-107">Crie um novo objeto de [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3f603-107">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f603-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3f603-108">Prerequisites</span></span>
<span data-ttu-id="3f603-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3f603-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3f603-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f603-111">Permission type</span></span>|<span data-ttu-id="3f603-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3f603-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f603-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f603-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f603-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f603-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3f603-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f603-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f603-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f603-116">Not supported.</span></span>|
|<span data-ttu-id="3f603-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f603-117">Application</span></span>|<span data-ttu-id="3f603-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f603-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f603-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f603-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3f603-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f603-120">Request headers</span></span>
|<span data-ttu-id="3f603-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3f603-121">Header</span></span>|<span data-ttu-id="3f603-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3f603-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f603-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f603-123">Authorization</span></span>|<span data-ttu-id="3f603-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f603-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f603-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3f603-125">Accept</span></span>|<span data-ttu-id="3f603-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f603-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f603-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f603-127">Request body</span></span>
<span data-ttu-id="3f603-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkApp.</span><span class="sxs-lookup"><span data-stu-id="3f603-128">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="3f603-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidForWorkApp.</span><span class="sxs-lookup"><span data-stu-id="3f603-129">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="3f603-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f603-130">Property</span></span>|<span data-ttu-id="3f603-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f603-131">Type</span></span>|<span data-ttu-id="3f603-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f603-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f603-133">id</span><span class="sxs-lookup"><span data-stu-id="3f603-133">id</span></span>|<span data-ttu-id="3f603-134">String</span><span class="sxs-lookup"><span data-stu-id="3f603-134">String</span></span>|<span data-ttu-id="3f603-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3f603-135">Key of the entity.</span></span> <span data-ttu-id="3f603-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3f603-137">displayName</span></span>|<span data-ttu-id="3f603-138">String</span><span class="sxs-lookup"><span data-stu-id="3f603-138">String</span></span>|<span data-ttu-id="3f603-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3f603-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3f603-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-141">description</span><span class="sxs-lookup"><span data-stu-id="3f603-141">description</span></span>|<span data-ttu-id="3f603-142">String</span><span class="sxs-lookup"><span data-stu-id="3f603-142">String</span></span>|<span data-ttu-id="3f603-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f603-143">The description of the app.</span></span> <span data-ttu-id="3f603-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3f603-145">publisher</span></span>|<span data-ttu-id="3f603-146">String</span><span class="sxs-lookup"><span data-stu-id="3f603-146">String</span></span>|<span data-ttu-id="3f603-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f603-147">The publisher of the app.</span></span> <span data-ttu-id="3f603-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3f603-149">largeIcon</span></span>|[<span data-ttu-id="3f603-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3f603-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3f603-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="3f603-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3f603-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f603-153">createdDateTime</span></span>|<span data-ttu-id="3f603-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f603-154">DateTimeOffset</span></span>|<span data-ttu-id="3f603-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f603-155">The date and time the app was created.</span></span> <span data-ttu-id="3f603-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f603-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3f603-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f603-158">DateTimeOffset</span></span>|<span data-ttu-id="3f603-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3f603-159">The date and time the app was last modified.</span></span> <span data-ttu-id="3f603-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3f603-161">isFeatured</span></span>|<span data-ttu-id="3f603-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f603-162">Boolean</span></span>|<span data-ttu-id="3f603-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3f603-164">privacyInformationUrl</span></span>|<span data-ttu-id="3f603-165">String</span><span class="sxs-lookup"><span data-stu-id="3f603-165">String</span></span>|<span data-ttu-id="3f603-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3f603-166">The privacy statement Url.</span></span> <span data-ttu-id="3f603-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3f603-168">informationUrl</span></span>|<span data-ttu-id="3f603-169">String</span><span class="sxs-lookup"><span data-stu-id="3f603-169">String</span></span>|<span data-ttu-id="3f603-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3f603-170">The more information Url.</span></span> <span data-ttu-id="3f603-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-172">owner</span><span class="sxs-lookup"><span data-stu-id="3f603-172">owner</span></span>|<span data-ttu-id="3f603-173">String</span><span class="sxs-lookup"><span data-stu-id="3f603-173">String</span></span>|<span data-ttu-id="3f603-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3f603-174">The owner of the app.</span></span> <span data-ttu-id="3f603-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-176">developer</span><span class="sxs-lookup"><span data-stu-id="3f603-176">developer</span></span>|<span data-ttu-id="3f603-177">String</span><span class="sxs-lookup"><span data-stu-id="3f603-177">String</span></span>|<span data-ttu-id="3f603-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f603-178">The developer of the app.</span></span> <span data-ttu-id="3f603-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-180">Observações</span><span class="sxs-lookup"><span data-stu-id="3f603-180">notes</span></span>|<span data-ttu-id="3f603-181">String</span><span class="sxs-lookup"><span data-stu-id="3f603-181">String</span></span>|<span data-ttu-id="3f603-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f603-182">Notes for the app.</span></span> <span data-ttu-id="3f603-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="3f603-184">uploadState</span></span>|<span data-ttu-id="3f603-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3f603-185">Int32</span></span>|<span data-ttu-id="3f603-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="3f603-186">The upload state.</span></span> <span data-ttu-id="3f603-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="3f603-188">publishingState</span></span>|[<span data-ttu-id="3f603-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3f603-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3f603-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f603-190">The publishing state for the app.</span></span> <span data-ttu-id="3f603-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="3f603-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3f603-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3f603-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3f603-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3f603-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3f603-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3f603-194">isAssigned</span></span>|<span data-ttu-id="3f603-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f603-195">Boolean</span></span>|<span data-ttu-id="3f603-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="3f603-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3f603-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3f603-198">roleScopeTagIds</span></span>|<span data-ttu-id="3f603-199">String collection</span><span class="sxs-lookup"><span data-stu-id="3f603-199">String collection</span></span>|<span data-ttu-id="3f603-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="3f603-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3f603-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f603-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f603-202">packageId</span><span class="sxs-lookup"><span data-stu-id="3f603-202">packageId</span></span>|<span data-ttu-id="3f603-203">String</span><span class="sxs-lookup"><span data-stu-id="3f603-203">String</span></span>|<span data-ttu-id="3f603-204">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="3f603-204">The package identifier.</span></span>|
|<span data-ttu-id="3f603-205">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="3f603-205">appIdentifier</span></span>|<span data-ttu-id="3f603-206">String</span><span class="sxs-lookup"><span data-stu-id="3f603-206">String</span></span>|<span data-ttu-id="3f603-207">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="3f603-207">The Identity Name.</span></span>|
|<span data-ttu-id="3f603-208">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3f603-208">usedLicenseCount</span></span>|<span data-ttu-id="3f603-209">Int32</span><span class="sxs-lookup"><span data-stu-id="3f603-209">Int32</span></span>|<span data-ttu-id="3f603-210">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="3f603-210">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="3f603-211">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3f603-211">totalLicenseCount</span></span>|<span data-ttu-id="3f603-212">Int32</span><span class="sxs-lookup"><span data-stu-id="3f603-212">Int32</span></span>|<span data-ttu-id="3f603-213">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="3f603-213">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="3f603-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3f603-214">appStoreUrl</span></span>|<span data-ttu-id="3f603-215">String</span><span class="sxs-lookup"><span data-stu-id="3f603-215">String</span></span>|<span data-ttu-id="3f603-216">Tocar para a URL do aplicativo de repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="3f603-216">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="3f603-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f603-217">Response</span></span>
<span data-ttu-id="3f603-218">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f603-218">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f603-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f603-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f603-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f603-220">Request</span></span>
<span data-ttu-id="3f603-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f603-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 876

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="3f603-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f603-222">Response</span></span>
<span data-ttu-id="3f603-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f603-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1048

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




