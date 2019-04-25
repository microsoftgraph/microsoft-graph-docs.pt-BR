---
title: Revisões de acesso ao Azure AD
description: Você pode usar as revisões do Azure AD Access para configurar revisões de acesso de uso único ou recorrente para atestado dos direitos de acesso do usuário.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 212af4ad8519f7ec54fb56ceffee0a0d4de16027
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544106"
---
# <a name="azure-ad-access-reviews"></a>Revisões de acesso ao Azure AD

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar as [revisões do Azure ad Access](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) para configurar revisões de acesso de uso único ou recorrente para atestado dos direitos de acesso do usuário.

Cenários de cliente típicos para revisões de acesso de associações de grupo e acesso de aplicativo são:
   
- Os clientes podem revisar e certificar o acesso de usuário convidado usando revisões de acesso de seu acesso a aplicativos e associações de grupos. Os revisores podem usar os insights fornecidos para decidir de forma eficiente se os convidados devem ter acesso contínuo.
      
- Os clientes podem analisar e certificar o acesso do funcionário aos aplicativos e às associações de grupo com as revisões do Access.
   
- Os clientes podem coletar controles de revisão de acesso em programas que são relevantes para a sua organização para rastrear as revisões de conformidade ou aplicativos sensíveis a riscos.

Há também um recurso relacionado para os clientes revisar e certificar as atribuições de função de usuários administrativos atribuídos às funções do Azure AD, como administrador global ou funções de assinatura do Azure.  Esse recurso está incluído no [Gerenciamento de identidade privilegiaDo do Azure ad](privilegedidentitymanagement-root.md).

Observe que o recurso de revisões de acesso, incluindo a API, está incluído no Azure AD Premium P2. 

## <a name="methods"></a>Métodos

Veja a seguir a lista de métodos fornecidos pelas revisões de acesso do Azure AD.  

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Obtenha uma revisão do Access com uma ID específica. |
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Criar um novo accessReview. |
|[Excluir accessReview](../api/accessreview-delete.md) | Nenhum.   | Excluir um accessReview. |
|[Atualizar accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Atualizar um accessReview. |
|[Listar revisores do accessReview](../api/accessreview-listreviewers.md) |      [](useridentity.md) coleção UserIdentity| Obter os revisores de um accessReview. |
|[Adicionar revisor accessReview](../api/accessreview-addreviewer.md) |      Nenhum.   |   Adicionar um revisor a um accessReview. |
|[Remover revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum.  |   Remover um revisor de um accessReview. |
|[Listar decisões accessReview](../api/accessreview-listdecisions.md) |      coleção [accessReviewDecision](accessreviewdecision.md)| Obtenha as decisões de um accessReview.|
|[Listar minhas decisões do accessReview](../api/accessreview-listmydecisions.md) |     coleção [accessReviewDecision](accessreviewdecision.md)| Como revisor, obtenha as minhas decisões de um accessReview.|
|[Enviar lembrete accessReview](../api/accessreview-sendreminder.md) |        Nenhum.   |   Envie um lembrete para os revisores de um accessReview. |
|[Parar accessReview](../api/accessreview-stop.md) |     Nenhum.   |   Parar um accessReview. |
|[Redefinir decisões do accessReview](../api/accessreview-reset.md) |     Nenhum.   |   ReDefina as decisões em um accessReview em andamento.|
|[Aplicar decisões accessReview](../api/accessreview-apply.md) |     Nenhum.   |   Aplique as decisões de um accessReview concluído.|
|[Listar businessFlowTemplates](../api/businessflowtemplate-list.md) | coleção [businessFlowTemplate](businessflowtemplate.md)| Obtenha os modelos de fluxo de negócios apropriados para as revisões do Access.|
|[Criar programa](../api/program-create.md) |   [programa](program.md)   |   Criar um novo programa.|
|[Excluir programa](../api/program-delete.md) |   Nenhum.   |   Excluir um programa.|
|[Listar programas](../api/program-list.md) |  coleção [Program](program.md)|   Obtenha uma coleção de todos os programas.|
|[Listar programControls de um programa](../api/program-listcontrols.md) |      coleção [programControl](programcontrol.md)| Obter uma coleção de controles de um programa.|
|[Programa de atualização](../api/program-update.md) |   [programa](program.md)|  Atualizar um programa.|
|[Criar programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Adicionar um programControl a um programa.|
|[Excluir programControl](../api/programcontrol-delete.md) |     Nenhum.   |   Remover um programControl de um programa.|
|[Listar programControls](../api/programcontrol-list.md) | coleção [programControl](programcontrol.md)| Listar controles em todos os programas no locatário.|
|[Listar programControlTypes](../api/programcontroltype-list.md) | coleção [programControlType](programcontroltype.md)| Listar tipos de controle de programa. |


## <a name="see-also"></a>Confira também

- [Como um administrador pode gerenciar o acesso do usuário com as revisões do Azure AD Access](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Como um administrador pode gerenciar o acesso de convidados com as revisões do Azure AD Access](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [Como um administrador pode gerenciar programas e controles para revisões do Azure AD Access](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviews-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
