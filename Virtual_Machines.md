# Teoria de Màquines Virtuals

Les màquines virtuals (VM) són sistemes que permeten executar diferents entorns de sistema operatiu i aplicacions de forma aïllada sobre el mateix maquinari físic. La idea central d'una màquina virtual és simular un sistema complet (incloent-hi el sistema operatiu) dins d'un entorn virtual, fent que sembli com si estigués treballant en un maquinari dedicat, quan en realitat està compartint recursos físics amb altres VM en un mateix servidor o ordinador. Això permet aprofitar millor els recursos i millorar la flexibilitat i la seguretat del sistema.

## Components i Funcionament

1. **Hypervisor (Monitor de màquina virtual)**: És el component clau que permet la virtualització. Actua com a capa d'abstracció entre el maquinari físic i les màquines virtuals. Hi ha dos tipus principals:
   - **Hypervisor de Tipus 1 (bare-metal)**: S'executa directament sobre el maquinari físic (exemples: VMware ESXi, Microsoft Hyper-V).
   - **Hypervisor de Tipus 2 (hosted)**: Funciona sobre un sistema operatiu existent (exemples: VirtualBox, VMware Workstation).

2. **Màquina Virtual (VM)**: Cada VM actua com un ordinador independent, amb el seu propi sistema operatiu i aplicacions. Està configurada amb recursos com CPU, memòria, disc dur i xarxa, que són proporcionats pel hypervisor.

## Avantatges

- **Eficiència de Recursos**: Les VM permeten utilitzar un mateix maquinari per a múltiples sistemes operatius, maximitzant l'ús de CPU, memòria i emmagatzematge.
- **Aïllament**: Les màquines virtuals estan aïllades unes de les altres, cosa que millora la seguretat i permet que si una VM falla o és atacada, les altres no es vegin afectades.
- **Flexibilitat i Portabilitat**: Les VM es poden moure fàcilment entre diferents servidors o dispositius físics.
- **Escalabilitat**: És fàcil afegir o eliminar VM en funció de les necessitats sense alterar el maquinari físic.

## Desavantatges

- **Consum de Recursos**: Cada màquina virtual consumeix recursos del sistema, i la sobrecàrrega de moltes VM pot fer que el rendiment disminueixi.
- **Complexitat en la Gestió**: La gestió i manteniment de moltes màquines virtuals pot requerir una gran quantitat de recursos administratius.
- **Dependència del Hypervisor**: Una fallada en el hypervisor pot afectar totes les màquines virtuals que gestiona.

## Aplicacions Pràctiques

- **Proves i Desenvolupament**: Els desenvolupadors poden utilitzar màquines virtuals per provar aplicacions en diferents sistemes operatius.
- **Consolidació de Servidors**: Les organitzacions utilitzen VM per combinar diferents aplicacions i serveis en menys servidors físics.
- **Entorns d'Aïllament**: Les VM són útils per executar entorns aïllats per a tasques que podrien ser insegures o experimentar fallades.

---

Les màquines virtuals són una part essencial de la infraestructura moderna en les TIC, sobretot en el camp de la **computació al núvol** (cloud computing), gràcies a la seva versatilitat i eficiència.
