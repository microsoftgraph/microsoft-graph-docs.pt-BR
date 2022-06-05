---
author: besiler
ms.topic: include
ms.date: 05/11/2022
ms.localizationpriority: medium
ms.openlocfilehash: 8d04a2787953278a40bf231cb9b6db117a67ebb5
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898971"
---
<!-- markdownlint-disable MD041-->

### <a name="viewing-applied-conditional-access-ca-policies-in-sign-ins"></a>Exibindo políticas de AC (acesso condicional) aplicadas em entradas
As políticas de AC aplicadas listadas na propriedade **appliedConditionalAccessPolicies** só estão disponíveis para usuários e aplicativos com funções que permitem ler dados de acesso [condicional](../resources/appliedconditionalaccesspolicy.md). Se um usuário ou aplicativo tiver permissões para ler logs de entrada, mas não permissão para ler dados de acesso condicional, a propriedade **appliedConditionalAccessPolicies** na resposta será omitida. As seguintes funções do Azure AD concedem aos usuários permissões para exibir dados de acesso condicional:

+ Administrador global
+ Leitor global
+ Administrador de Segurança
+ Leitor de segurança
+ Administrador de Acesso Condicional

Os aplicativos devem ter pelo menos uma das seguintes permissões para ver objetos [appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) nos logs de entrada: 

+ Policy.Read.All
+ Policy.ReadWrite.ConditionalAccess
+ Policy.Read.ConditionalAccess

>**Nota:** Os usuários do Azure AD com quaisquer permissões podem ler os logs de entrada nos quais o usuário é o ator que está entrando. Esse recurso ajuda os usuários a detectar atividades inesperadas em suas contas. Os usuários não podem ler dados de AC de seus próprios logs, a menos que tenham uma das permissões de AC identificadas acima.
